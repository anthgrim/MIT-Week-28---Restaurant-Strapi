# Instructions

Hey guys I made the assignment work but it's a lot to follow along.

Steps:

1. Downgrade your node version to version 12

- You will need to install nvm using the following curl or wget command (make sure to use bash)

  ```bash
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.shLinks to an external site. | bash
  ```

- or the wget command from the nvm repo https://github.com/nvm-sh/nvmLinks to an external site.

2. After that you should see that your nvm is installed by running the following command => `command -v nvm`

- if you don't see anything, you need to execute the nvm manually by running these commands:

  ```bash
  export NVM_DIR="$HOME/.nvm"
  [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
  ```

3. After that run: `nvm install 12`

   - The strapi version being used is node 12 or node 14.... it's in the package.json of the strapi code

4. Check your node version with: `node -v` or `node --version` and you should see version 12 running
5. then using the same bash terminal navigate to your directory where the backend strapi code is located. Do the following commands one by one:

   ```bash
   cd Documents/MIT/restaurant-strapi/backend
   npm install
   npm run develop
   ```

6. then open a separate terminal, navigate to your nextjs directory, in my case was

   ```bash
   cd Documents/MIT/restaurant-strapi
   npm install
   npm run dev
   ```

7. open localhost:3000 and go to the sign up, try to sign up and you are good to go
   when adding the roles and permission make sure you check all the boxes to start using all the endpoints, otherwise is not gonna work when loading the restaurants in the ui
