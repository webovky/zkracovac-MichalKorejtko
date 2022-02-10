Start Flask
=========================

[flask]: https://flask.palletsprojects.com

Tento repositář má vám (i mě) usnadnit založení nového projektu
s frameworkem [Flask][].

Několik užitečných odkazů pro začátek
------------------------------------------

* [Explore Flask](https://exploreflask.com/)
* [The Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
---------------------------------------------------------------------------
* <https://github.com/pyvec/elsa>
* <https://github.com/smoqadam/PyFladesk>
* <https://github.com/ClimenteA/flaskwebgui>
* <https://elc.github.io/posts/executable-flask-pyinstaller/>
---------------------------------------------------------------------------
* [w3schools.com](https://www.w3schools.com/) ,[Jak psát web](https://www.jakpsatweb.cz/) 
* [Flask docs][flask],  [Flask Quick start](https://flask.palletsprojects.com/quickstart/)
* [Template Designer Documentation](https://jinja.palletsprojects.com/templates/)
* [Bábot](https://www.blabot.cz/)
* [Clker.com](http://www.clker.com/), [Commons](https://commons.wikimedia.org),
  [pixabay](https://pixabay.com/), [Unsplash](https://unsplash.com/)
---------------------------------------------------------------------------

 ... jak na to?
 ------------------------

Zde najdete základní adresářovou strukturu pro aplikaci ve 
[Flasku][flask]

0. Dejme tomu že začínám nový projekt. Bude se jmenovat třeba *Foo*.
Můžete si [forknout](htts://help.github.com/articles/fork-a-repo/)
nebo prostě jen 
[naklonovat](https://help.github.com/articles/cloning-a-repository/)
tento repositář:


```bash
git clone --depth 1 https://github.com/spseol/startflask.git Foo
cd Foo
```
Repositář obsahuje skript **`start.sh`**, který vše další udělá za vás.
Pokud chcete mít kontrolu, můžete pokračovat a všechno si pěkně udělat růčo.

1. Vytvořím si [virtuální prostředí](https://virtualenv.pypa.io/en/stable/)
   právě pro aplikaci *Foo*.:

```bash
python3 -m venv .venv-foo
```

2. Virtuální prostředí si aktivuji:

```bash
source .venv-foo/bin/activate
```
nebo na Windows:
```
.venv-foo\Scripts\activate

```

3. Do virtuálního prostředí nainstaluji potřebné moduly:

```bash
pip install -r requirements.txt
```
nebo ručně nestručně:

```bash
pip install flask flask-socketio
pip install flask-mail flask-misaka
pip install psycopg2 pony
```


4. A teď stačí spustit vývojový server:

```
flask run
```
