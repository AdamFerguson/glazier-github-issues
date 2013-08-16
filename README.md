glazier-github-issues
=====================

A card for viewing github issues for a repository.

## Adding to glazier

    # in `glazier/cards/`
    ln -s your/path/to/glazier-github-issues github-issues

    # in `glazier/`
    grunt ingestCards

    # in `glazier/glazier-server/`
    bundle exec rails console

    # add the Pane to the dashboard of your choosing
    db = Dashboard.where(repository: 'emberjs/ember.js').first
    db.add_pane('glazier-github-issues')


## Running Tests
  grunt autotest

  # view in browser
  open dist/dev/github-issues/test.html
