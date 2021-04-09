# cultivaPy

Plataforma de conexión entre pequeño productor agrícola y cliente final

#### URL

https://cultivapy.org

## Requirements

- Python 3.6+
- PostGIS 3.0+
- PostgreSQL 11+
- Gettext 0.19+

## Install

```
git clone git@github.com:enzoama95/cultivapy.git
cd cultivapy
python3 -m venv cultivapy-env
source cultivapy-env/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
cp conf/.env.example conf/.env # you should edit this file with your configuration
create database with the name that used in ".env" file
./manage.py migrate
./manage.py compilemessages
./manage.py runserver
```

We use `django-pipeline` to handle CSS/JS assests, and this library requires `yuglify`. To install `yuglify`, issue the following:

```
npm -g install yuglify
```

The above command assumes that [NPM](https://www.npmjs.com/get-npm) is available.


## Author

- Enzo Amarilla https://github.com/enzoama95

## Contributors / Thanks

- Marcelo Elizeche Landó https://github.com/melizeche




## License

This project is licensed under the terms of the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details
