# Word Frequency

A Flask app that calculates word-frequency pairs based on the text from a given URL

Flask by example from Real Python:
https://realpython.com/blog/python/flask-by-example-part-1-project-setup/

Requirements
===
<pre><code>
redis-server
requiments.txt
</pre></code>

Install
===
<pre><code>
pip install -r requirements.txt
</pre></code>

Setup the database
===
<pre><code>
Create a dabase with name wordcount on PostgreSQL
python manage.py db init
python manage.py db migrate
python manage.py db upgrade
</pre></code>

Run
===
<pre></code>
Make sure redis-server is running
export APP_SETTINGS="config.DevelopmentConfig"
export DATABASE_URL="postgresql://localhost/wordcount_dev"
python worker.py
On other tab run:
python app.py
</pre></code>