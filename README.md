[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php)
# ci-miniconda
Docker image for building Python packages in Jenkins

Featuring:
* [Miniconda](https://conda.io/miniconda.html)
* [Pipenv](https://docs.pipenv.org/)
* [Twine](http://twine.readthedocs.io/en/latest/)

# Development
## Building the image
```
docker build -t ci-python .
```
## Running the image (for troubleshooting)
```
docker run -it -d --rm --name cp ci-python:latest
```

Then:
```
docker exec -it cp sh
```
