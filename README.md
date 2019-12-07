# The-Android-App-Market-on-Google-Play
The Android App Market on Google Play Dataset project for data engineering 

### Organization of the  project

The project has the following structure:

    repo/
      |- README.md
      |- code/
         |- due.py
      |- data/
         |- googleplaystore_user_reviews.csv
         |- googleplaystore.csv
         |- license.txt
      |- .gitignore
      |- android.ipynb
      |- LICENSE
      |- ipynb/
         |- ...


### Project Data

In this case, the project data is rather small, and recorded in csv
files.  Thus, it can be stored alongside the module code.  Even if the
data that you are analyzing is too large, and cannot be effectively
tracked with github, you might still want to store some data for
testing purposes.

Either way, you can create a `repo/data` folder in which you can
organize the data.



### Styling

It is a good idea to follow the PEP8 standard for code formatting. Common code
formatting makes code more readable, and using tools such as `flake8` (which
combines the tools `pep8` and `pyflakes`) can help make your code more readable,
avoid extraneous imports and lines of code, and overall keep a clean project
code-base.

Some projects include `flake8` inside their automated tests, so that every pull
request is examined for code cleanliness.

In this project, we have run `flake8` most (but not all) files, on
most (but not all) checks:

```
flake8 --ignore N802,N806 `find . -name *.py | grep -v setup.py | grep -v /doc/`
```

This means, check all .py files, but exclude setup.py and everything in
directories named "doc". Do all checks except N802 and N806, which enforce
lowercase-only names for variables and functions.

The `Makefile` contains an instruction for running this command as well:

    make flake8
### Licensing

MIT License 
### Git Configuration


- `.gitignore` -- specifies intentionally untracked files (such as
  compiled `*.pyc` files), which should not typically be committed to
  git (see `man gitignore`)

### For developers
Finally, you will probably want to change the copyright holder in the `LICENSE`
file to be you. You can also replace the text of that file, if it doesn't match
your needs.
