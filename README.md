# pgzero-indonesian

[![Join the chat at https://gitter.im/pgzero-indonesian/Lobby](https://badges.gitter.im/pgzero-indonesian/Lobby.svg)](https://gitter.im/pgzero-indonesian/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Docs translation in Indonesian of <https://github.com/lordmauve/pgzero>

## Build the Docs

This documentation is written in [reStructuredText](http://docutils.sourceforge.net/rst.html) and can be build with Sphinx. Make sure you have [Sphinx](http://www.sphinx-doc.org/en/master/usage/installation.html) installed. To build the docs to html, in project directory :

```bash
make html
```

The result available in `_build/html`. To see the result you can simply use any http server, such as python3 http.server

```bash
cd _build/html
python3 -m http.server
# Open browser and go to localhost:8000
```

## Contributing

Currently we are doing Translate Phase. Please read the [issue](https://github.com/mamat-rahmat/pgzero-indonesian/issues/1).

If you have something to discuss, chat us on gitter by clicking the badge above.

Steps to contribute :

1. Make sure the translation you want to create or fix isn't already taken by other contributor by looking at [issues](https://github.com/mamat-rahmat/pgzero-indonesian/issues) (both open/closed). If no one working on that, first create the issue. After that, you can continue the step.

2. Click “Fork” to create your own fork of the repository.

3. Clone this fork to your own computer:

   ```
   git clone git@github.com:yourusername/pgzero-indonesian.git
   ```

   Remember to change `yourusername` to your Github username.

4. Create a branch in which to do your changes. Pick a branch name that describes the change you want to make.

   ```
   git checkout -b my-new-branch master
   ```

5. Make the changes you want. Make sure you are satisfied with the result. To build the result, see [Building the Docs](#building-the-docs).

6. Add the files that you want to commit:

   ```
   git add myfile.rst
   ```

7. Commit the files with a clear commit message:

   ```
   git commit -m "Translate myfile.rst"
   ```

8. Push the commit back to your fork.

   ```
   git push --set-upstream origin my-new-branch
   ```

9. Go to the Github page for your fork, and click on the “Create pull request” button.