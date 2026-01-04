<div align="center">
<h1><a><b>Shortify</b></a></h1>
</div>

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Documentation and Usage](#documentation-and-usage)
- [Project Structure, Modifications and Best Practices](#project-structure-modifications-and-best-practices)
    - [Creating new API routes](#creating-new-api-routes)
    - [FastAPI Best Practices](#fastapi-best-practices)
- [Stack](#stack)

## Introduction

_Shortify_ is a fast, fully async and reliable URL shortener RESTful API built with Python and [FastAPI] framework.
It uses the open source [MongoDB] database for storing shortened URLs data and implements user registration via
OAuth2 JWT authentication.

## Features

- Dockerized and ready to be deployed.
- Fully async and non-blocking.
- Uses [FastAPI] framework for API development:
- Uses [MongoDB] as data store for users and shortened URLs.
- Extensible architecture for adding new API endpoints and services.
- Descriptive and well-documented code.
- OAuth2 (with hashed passwords and JWT tokens) based user authentication.
- Uses [Poetry] for dependency management.
- Automated code formatting and linting with [pre-commit] and [black].
- [CORS (Cross Origin Resource Sharing)](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) support.
- Pagination support for listing shortened URLs and users.
- Structured logging with [structlog].
- Correlation ID middleware for logging and tracing requests across services.
- Class-based API endpoints for better code organization and reducing duplication.
- Fully type annotated code for better IDE support and code quality.

## Requirements

Manual installation:

- Python 3.8 or higher.
- [Poetry] for dependency management.
- Up and running [MongoDB] instance (locally or remotely).

Using Docker:

- [Docker]
- [Docker-Compose]

## Stack

Frameworks and technologies used in _Shortify_

- [FastAPI] (Web framework)
- [structlog] (Logging)
- [MongoDB] (Database)
- [beanie] (ODM)
- [poetry] (Dependency Management)
- [pre-commit] (Git hook)
- [ruff] (Linter)
- [black] & [isort] (Formatter)
- [mypy] (Type checker)


[FastAPI]: https://github.com/tiangolo/fastapi "Modern, high-performance, web framework for building APIs with Python."
[MongoDB]: https://www.mongodb.com/ "General purpose, document-based, distributed database."
[Poetry]: https://python-poetry.org/ "Python dependency management and packaging made easy."
[pre-commit]: https://pre-commit.com/ "A framework for managing and maintaining multi-language pre-commit hooks."
[black]: https://github.com/psf/black "The uncompromising Python code formatter."
[GPL-3.0]: https://www.gnu.org/licenses/gpl-3.0.en.html "GNU General Public License v3.0"
[structlog]: https://www.structlog.org/en/stable/ "Structured logging for Python."
[logging]: https://docs.python.org/3/library/logging.html "Logging facility for Python."
[secrets]: https://docs.python.org/3/library/secrets.html "Generate secure random numbers for managing secrets."
[uvicorn]: https://www.uvicorn.org/ "The lightning-fast ASGI server."
[gunicorn]: https://gunicorn.org/ "A Python WSGI HTTP Server for UNIX."
[VSCode]: https://code.visualstudio.com/ "Redefined and optimized code editor for building and debugging modern web and cloud applications."
[fastapi-best-practices]: https://github.com/zhanymkanov/fastapi-best-practices "Opinionated list of best practices and conventions."
[full-stack-fastapi-postgresql]: https://github.com/tiangolo/full-stack-fastapi-postgresql "Full stack, modern web application generator. Using FastAPI, PostgreSQL as database, Docker, automatic HTTPS and more."
[pydantic]: https://github.com/pydantic/pydantic "Data parsing and validation using Python type hints."
[beanie]: <https://github.com/roman-right/beanie> "Python ODM for MongoDB."
[isort]: <https://github.com/PyCQA/isort> "A Python utility / library to sort imports."
[mypy]: https://github.com/python/mypy "Optional static typing for Python."
[ruff]: https://github.com/charliermarsh/ruff "An extremely fast Python linter, written in Rust."
[Docker]: https://github.com/docker/
[Docker-Compose]: https://github.com/docker/compose "Define and run multi-container applications with Docker."
