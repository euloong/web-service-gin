# Developing a RESTful API with Go and Gin

Using the [Go docs tutorial](https://go.dev/doc/tutorial/web-service-gin)

1. Run the app with `go run .`
2. In another terminal window, run the following `curl` commands to make requests to the web service:

    GET all albums

    ```bash
    $ curl http://localhost:8080/albums
    ```

    POST add new album

    ```bash
    $ curl http://localhost:8080/albums \
        --include \
        --header "Content-Type: application/json" \
        --request "POST" \
        --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
    ```

    GET album by `/id`

    ```bash
    $ curl http://localhost:8080/albums/2
    ```
