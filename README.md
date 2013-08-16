glazier-github-stars
====================

This card shows github users who have starred the current repository.


## Adding to glazier

    # in `glazier/cards/`
    ln -s your/path/to/glazier-github-stars github-stars

    # in `glazier/`
    grunt ingestCards

    # in `glazier/glazier-server/`
    bundle exec rails console

    # add the Pane to the dashboard of your choosing
    db = Dashboard.where(repository: 'emberjs/ember.js').first
    db.add_pane('glazier-github-stars')


## Running Tests
  grunt autotest

  # view in browser
  open dist/dev/github-stars/test.html
