# Main Purpose
- This project was created by me and its purpose is to prepare himself for his role as Frontend Software Engineer.
- Currently the company is using the stack:Go backend with graphql
  - Go backend
  - GraphQl
  - React frontend with Flow Typing
  - Electron app with web wrapper
- Thus this project will be a boilerplate that hooks all those together. 
- The backend comes from the boilerplate graphql-go. Please see License file for license usage.
- Hoping this is useful for someone out there looking to start a project as fast as possible :)


# Go Backend
- Since this is my first time working with a Go server I was following [this guide](https://dev.to/glyphack/introduction-to-graphql-server-with-golang-1npk) 
- Here is an excerpt describing the files
    - gqlgen.yml — The gqlgen config file, knobs for controlling the generated code.
    - generated.go — The GraphQL execution runtime, the bulk of the generated code.
    - models_gen.go — Generated models required to build the graph. Often you will override these with your own models. Still very useful for input types.
    - resolver.go — This is where your application code lives. generated.go will call into this to get the data the user has requested.
    -server/server.go — This is a minimal entry point that sets up an http.Handler to the generated GraphQL server. start the server with go run server.go and open your browser and you should see the graphql playground, So setup is right!
