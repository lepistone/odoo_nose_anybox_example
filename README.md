# run odoo unittests with anybox.recipe.odoo and nose

```bash
python2 bootstrap.py
bin/buildout

createdb any_db
bin/start_openerp -i sale --stop-after-init
bin/nosetests_odoo -- parts/odoo/addons/sale/tests
```
