# Testing and Publishing package on PyPI

## Upload to testpypi
pip install twine
twine upload --repository-url https://test.pypi.org/legacy/ dist/pyandy-0.1.0.tar.gz

pip install -i https://test.pypi.org/simple/ pyandy==0.0.1

# Upload to pypi
twine upload dist/*

pip install pyandy --user

# References
* https://betterscientificsoftware.github.io/python-for-hpc/tutorials/python-pypi-packaging/#uploading-to-testpypi