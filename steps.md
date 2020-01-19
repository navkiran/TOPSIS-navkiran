python3 setup.py bdist_wheel
python3 setup.py bdist_wheel sdist
python3 -m twine upload dist/*
