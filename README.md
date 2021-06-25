# Django and mongo-datatables

Fork from : [https://github.com/pjosols/django-and-mongo-datatables](https://github.com/pjosols/django-and-mongo-datatables)

A sample website that shows how to use mongo-datatables with Django. Checkout the models, urls, views, and the db.html template in the polls app.

----

## Install mongo-datatables

Install latest version of Mongo-datatables from git:

    git clone https://github.com/pauljolsen/mongo-datatables
    cd mongo-datatables/
    python3 setup.py install

## DataTables static files

This is what you need to download from [DataTables](https://datatables.net/download/)  Note, Editor is paid version. You can ignore if you don't want it.

#### Also, One can install the datatables using NPM

```
npm install --save jquery
npm install --save jszip
npm install --save pdfmake
npm install --save datatables.net-bs5
npm install --save datatables.net-editor-bs5
npm install --save datatables.net-autofill-bs5
npm install --save datatables.net-buttons-bs5
npm install --save datatables.net-colreorder-bs5
npm install --save datatables.net-datetime
npm install --save datatables.net-fixedcolumns-bs5
npm install --save datatables.net-fixedheader-bs5
npm install --save datatables.net-keytable-bs5
npm install --save datatables.net-responsive-bs5
npm install --save datatables.net-rowgroup-bs5
npm install --save datatables.net-rowreorder-bs5
npm install --save datatables.net-scroller-bs5
npm install --save datatables.net-searchbuilder-bs5
npm install --save datatables.net-searchpanes-bs5
npm install --save datatables.net-select-bs5
```

After installing NPM update polls/templates/polls/db.html to include right path for datatables.min.js and editor

```
<script type="text/javascript" src="{% static '/DataTables/datatables.min.js' %}"></script>
<script type="text/javascript" src="{% static '/DataTables/Editor-2.0.4/js/dataTables.editor.js' %}"></script>
```

![datatables static files](datatables_static_files.jpg)
