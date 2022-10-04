# tmsb_api

Это проект для получения базы фильмов, их сортировки и поиска фильмов по ключевым словам.

## Как он работает:

1. Вы скачиваете 1000 книг с Api сайта `https://api.themoviedb.org` и получаете их в виде JSON. Используя следующий скрипт.
```python
python make_own_db.py
```
2. С помощью следующего скрипта вы можете скачать одну книгу по ID из базы книг по Api.
```python
python hello_api_TMDB.py
```
3. Что бы найти все фильмы, где в названии встречаются запрошенное ключевое слово и вывести их в отсортированном списке, используйте скрипт ниже.
```python
python search_in_db.py
```
4. Следующий скрипт вернет 8мь фильмов с наивысшим рейтингом. Из совпавших по ключевому слову.
```python
python find_similar.py
```

5. Остальные скрипты икрают вспомогательную роль для первых 4-х, `own_db_helpers.py` - данный скрипт проверяет если путь до файла существует, то записывает его как словарь питона и возвращает
   А второй скрипт `tmdb_helpers.py` - проверяет наличие ключа Api, а также проверяют и получает книги для последующего сохранения как словарь Python.


## Установка

Используйте данную инструкцию как установить этот скрипт


1. Установить

```python
git clone https://github.com/Maxim-Pekov/tmdb_api
python -m venv venv
```
2. Activate venv    
```python
.\venv\Scripts\activate         #windows
source ./venv/bin/activate      #Linux, Mac  
```
3. Go to the `./tmdb_api` directory
4. Install requirements
```python
pip install -r requirements.txt
```

