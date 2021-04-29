# Instruções para interagir com o PyLab via console

Para interagir com o PyLab usando o console interativo do Python:
Abra um prompt do Python partindo da mesma pasta onde se encontra o módulo PyLab.py
Digite a linha abaixo para importar o módulo:

```python
>>> import PyLab
```

Iniciar um novo objeto para se comunicar com o lab:

```python
>>> lab = PyLab.Lab(host='IP')
```

Registrar um novo usuário (necessário apenas uma vez):

```python
>>> lab.Register('user','email')
```

GUARDE A CHAVE DE API!!!
Caso precise efetuar login novamente, apenas crie o objeto lab e passe a chave de API:

```python
>>> lab = PyLab.Lab(host='IP', apikey=<chave_de_api>)
```

Ajuda para interagir com o PyLab:

```python
>>> lab.Help()
```

Para usar o módulo de forma automatizada a fim de responder às questões do PyLab, veja o arquivo PyLabSolver.py