# ReactTS-Django-integration template

After cloning the repo, `cd` into it with

```
cd ReactTS-with-Django
```

Once you're inside, run

```
pip install -r requirements.txt
```

This will install all the dependencies from the `requirements.txt` file into your current environment. (Using a virtualenv is highly recommended)

Next, `cd` into the Reactfrontend folder with

```
cd Reactfrontend
```

and run

```
npm install
```

This will install all the dependencies in the `package.json` file and create a folder named `node_modules`.
Next, run

```
npm run build
```

to build the project for production. Once done with the installation and build process, `cd` back to the base directory using

```
cd ..
```

Finally, run

```
python manage.py run server
```

Et voila! You just integrated your react code with django. You should now be able to see the boilerplate template for React + Vite in the browser.

Note: Every time you make changes to your frontend code, you'll need to run `npm run build` since we're serving the static files from the dist folder(or the build folder in the case of CRA).
