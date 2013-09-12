=======================================================================
 sched: Example Application for Packt's 2013 Flask book by Ron DuPlain
=======================================================================

To run this project, create a virtualenv with Python 2.7 or Python 3.3+ as
described in the first section of the book, activate that virtualenv, then set
up your application with these commands::

    pip install -r stable.txt
    python manage.py create_tables

Create a user in the Python shell::

    python manage.py shell

By executing this Python code in the interactive interpreter::

    from sched.app import db, User
    user = User(email='you@example.com', password='secret')
    db.session.add(user)
    db.session.commit()

Start the development server with::

    python manage.py runserver

Point your web browser to http://localhost:5000/appointments/.
Login with authentication credentials you used when creating the user.

*Flask Web Development* by Ron DuPlain through Packt, 2013:
http://www.packtpub.com/flask-web-development/book

See the `Flask mailing list discussion for context
<http://librelist.com/browser/flask/2013/8/28/flask-web-development-book-now-available-through-packt/>`_.
