# Back-end

### Flask backend
`cd backend/`

### Installation
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

#### To activate next time
`source venv/bin/activate`

### Configurations

The config.py for our database manager (postgreSQL)

```python
SQLALCHEMY_DATABASE_URI = 'postgresql+psycopg2://{user}:{pw}@{url}/{db}'.format(user='postgres', pw='root',
                                                                                  url='127.0.0.1', db='soft_eng_db')
```

### Run
`python3 run.py or python run.py`

For testing our HTTP requests we used Postman

### HTTPS

For self-signed-certificate in the script run.py:

```python
if __name__ == "__main__":
    app.run(host='127.0.0.1', debug=True, port='5000', ssl_context='adhoc')
```

### Unit & Functional Testing
`cd tests/` and 
`py.test -sv`