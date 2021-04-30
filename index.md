<head>
<!-- Ajax call -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython.js" integrity="sha256-rA89wPrTJJQFWJaZveKW8jpdmC3t5F9rRkPyBjz8G04=" crossorigin="anonymous"></script> 

<script src="https://cdnjs.cloudflare.com/ajax/libs/brython/3.8.8/brython_stdlib.js" integrity="sha256-Gnrw9tIjrsXcZSCh/wos5Jrpn0bNVNFJuNJI9d71TDs=" crossorigin="anonymous"></script> 
 <!-- Ajax call -->
</head>
<body onload="brython()">
    <h1>Get a joke</h1>

    <button id="joke-btn">Get Joke</button>
    <div id="joke" class="card">Click the "get joke" button</div>

    <!-- Ajax call -->
    <script type="text/python" id="script13">
        from browser import document, ajax

        url = 'https://api.chucknorris.io/jokes/random'

        def on_complete(req):
            import json
            data = json.loads(req.responseText)
            joke = data['value']
            document['joke'].text = joke

        def get_joke(e):
            req = ajax.ajax()
            req.open('GET', url, True)
            req.bind('complete', on_complete)
            document['joke'].text = 'Loading...'
            req.send()

        document['joke-btn'].bind('click', get_joke)
    </script>

</body>
