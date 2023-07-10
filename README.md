# Cellular Automata Pattern Database

This is the repository for the Database of Cellular Automata Patterns.

## Running the Database

This is the workflow for prototyping the database schema.
TODO: Update this when the database goes live.

1. Setup

   -  Prerequisites
      -  [Node.js](https://nodejs.org)
      -  [Yarn](https://yarnpkg.com/)
      -  [Python](https://python.org)
   -  Setup Project
      ```sh
      git clone https://github.com/conwaylife-dev/conwaylifedb
      yarn install
      cp .env.example .env # This should be handled differently in production
      ```

2. Import data from file and run the dev server

   ```sh
   yarn strapi import -f ${filename}
   yarn develop
   ```

3. Edit the schema and add data with the admin page.

   -  A script that autoimports data in bulk is planned after the schema is set.

4. Save your work

   ```sh
   # TODO: Do encrypt once the project contains user data or has private data for some reason
   yarn strapi export --no-encrypt
   ```

5. Share the prototype database.
