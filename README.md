# MovieApp
Project to practice React using create-react-app

## Build Production
1. Go to project folder

2. Add this to **package.json**:
    ```text
       "homepage": "http://<your github id>.github.io/movie_app"
    ```
    
3. Follow below lines:
    ```bash
    $ yarn build
    # yarn add --dev gh-pages
    ```
    
4. Add the following script in your **package.json**:
    ```text
       // ...
       "script": {
           // ...
           "predeploy": "npm run build",
           "deploy": "gh-pages -d build"
       }
    ```

5. Then run:
    ```bash
    $ yarn run deploy
    ```