# Django REST Framework (DRF) Professional Roadmap

_A professional, actionable roadmap for mastering Django REST Framework in 21 days. Each day covers core DRF concepts, best practices, and includes targeted "homework" for practical mastery._

---

## Table of Contents

- [Overview](#overview)
- [Roadmap Table (21 Days)](#roadmap-table-21-days)
- [Daily Breakdown](#daily-breakdown)
- [Resources](#resources)

---

## Overview

This roadmap is designed for developers looking to master Django REST Framework (DRF) with a structured, daily approach. Each day provides focused learning objectives and practical homework assignments to reinforce understanding.

---

## Roadmap Table (21 Days)

| Day | Topic                                   | Key Objectives                                              | Homework / Practice                        |
|-----|-----------------------------------------|-------------------------------------------------------------|--------------------------------------------|
| 1   | DRF Overview & Setup                    | Intro, Install DRF, Project Setup                           | Create Django project, install DRF         |
| 2   | DRF App Structure & Settings            | App structure, settings.py, INSTALLED_APPS                  | Configure DRF in settings.py               |
| 3   | Serializers: Basics                     | Serializer classes, basic serialization                     | Create simple serializer                   |
| 4   | Models & Serializers: Nested            | ModelSerializers, nested serializers                        | Build related models & serializers         |
| 5   | Views: APIView & Response               | APIView, Response, request/response cycle                   | Write basic APIView                        |
| 6   | Views: Generics                         | Generic views: ListAPIView, RetrieveAPIView, etc.           | Implement generic views                    |
| 7   | Routers & ViewSets                      | ViewSets, routers, URL conf                                 | Refactor views using ViewSets              |
| 8   | CRUD Operations                         | Full CRUD: Create, Read, Update, Delete                     | Implement all CRUD endpoints               |
| 9   | Authentication: Basics                  | DRF Auth, TokenAuth, SessionAuth                            | Protect endpoints with authentication      |
| 10  | Permissions & Throttling                | Permissions, custom permissions, throttling                 | Write custom permission class              |
| 11  | Filtering & Searching                   | Filtering, search, ordering                                 | Add ordering & search to endpoints         |
| 12  | Pagination                             | DRF pagination styles                                       | Add pagination to list views               |
| 13  | Advanced Serializers                    | SerializerMethodField, custom validation                    | Add custom validation to serializers       |
| 14  | Relationships & Hyperlinked             | HyperlinkedModelSerializer, related fields                  | Use hyperlinked relationships              |
| 15  | Testing APIs                           | APIClient, APIRequestFactory, writing tests                 | Write tests for your API endpoints         |
| 16  | Documentation: Swagger, Redoc           | auto-generated docs with drf-yasg or drf-spectacular        | Add Swagger/Redoc to project               |
| 17  | Permissions: Object-level               | Object-level permissions, custom logic                      | Implement object-level permissions         |
| 18  | Advanced Topics I: Signals, Hooks       | DRF signals, hooks, pre/post_save                           | Use signals for post-creation processing   |
| 19  | Advanced Topics II: Caching, RateLimit  | Caching, API rate limiting                                  | Add caching to your API                    |
| 20  | Deploying DRF APIs                      | Deploy with Gunicorn/UWSGI, Nginx, environment variables    | Deploy to Heroku, DigitalOcean, or similar |
| 21  | Real Project & Review                   | Build a mini project, review concepts                       | Complete and document a capstone project   |

---

## Daily Breakdown

### Day 1: DRF Overview & Setup
- **Objective**: Understand REST, install Django, DRF.
- **Homework**:  
   - Install Django and DRF.  
   - Setup new project:  
     ```bash
     pip install django djangorestframework
     django-admin startproject drf_project
     ```

### Day 2: DRF App Structure & Settings
- **Objective**: Understand Django app structure, configure DRF.
- **Homework**:  
   - Create new app: `python manage.py startapp api`
   - Add to `INSTALLED_APPS` in `settings.py`:
     ```python
     INSTALLED_APPS = [
         # ...
         'rest_framework',
         'api',
     ]
     ```

### Day 3: Serializers - Basics
- **Objective**: Learn about serializers.
- **Homework**:  
   - Create a simple serializer in `api/serializers.py`.

### Day 4: Models & Serializers - Nested
- **Objective**: ModelSerializers, nested data.
- **Homework**:  
   - Add related models, create nested serializers.

### Day 5: Views - APIView & Response
- **Objective**: Use APIView, handle requests/responses.
- **Homework**:  
   - Write a basic APIView in `api/views.py`.

### Day 6: Views - Generic Views
- **Objective**: Use DRF generic views.
- **Homework**:  
   - Implement ListAPIView, RetrieveAPIView.

### Day 7: Routers & ViewSets
- **Objective**: Use routers & ViewSets.
- **Homework**:  
   - Refactor views using ViewSets and routers.

### Day 8: CRUD Operations
- **Objective**: Create full CRUD endpoints.
- **Homework**:  
   - Implement Create, Read, Update, Delete endpoints.

### Day 9: Authentication - Basics
- **Objective**: Learn authentication in DRF.
- **Homework**:  
   - Protect endpoints using TokenAuthentication.

### Day 10: Permissions & Throttling
- **Objective**: Permissions and throttling.
- **Homework**:  
   - Write and apply custom permissions.

### Day 11: Filtering & Searching
- **Objective**: Add filtering, search, and ordering.
- **Homework**:  
   - Add search and ordering to endpoints.

### Day 12: Pagination
- **Objective**: Use DRF pagination.
- **Homework**:  
   - Add pagination to list endpoints.

### Day 13: Advanced Serializers
- **Objective**: Custom fields & validation.
- **Homework**:  
   - Use `SerializerMethodField`, write custom validator.

### Day 14: Relationships & Hyperlinked Serializers
- **Objective**: Model relationships, use hyperlinked serializers.
- **Homework**:  
   - Refactor to `HyperlinkedModelSerializer`.

### Day 15: Testing APIs
- **Objective**: Test APIs with APIClient.
- **Homework**:  
   - Write unit tests for endpoints.

### Day 16: Documentation - Swagger/Redoc
- **Objective**: Auto-generate API docs.
- **Homework**:  
   - Integrate Swagger or Redoc using drf-yasg or drf-spectacular.

### Day 17: Permissions - Object-level
- **Objective**: Object-level permissions.
- **Homework**:  
   - Implement and apply object-level permissions.

### Day 18: Advanced Topics I - Signals, Hooks
- **Objective**: Use signals and hooks in DRF.
- **Homework**:  
   - Add a signal for post-save logic.

### Day 19: Advanced Topics II - Caching, Rate Limiting
- **Objective**: Improve performance.
- **Homework**:  
   - Add caching and rate limiting.

### Day 20: Deploying DRF APIs
- **Objective**: Deploy DRF project.
- **Homework**:  
   - Deploy on Heroku, DigitalOcean, etc.

### Day 21: Real Project & Review
- **Objective**: Build a mini-project, review all concepts.
- **Homework**:  
   - Complete a small REST API project and document it.

---

## Resources

- [Official DRF Docs](https://www.django-rest-framework.org/)
- [DRF Tutorial](https://www.django-rest-framework.org/tutorial/quickstart/)
- [DRF - Advanced Features](https://www.django-rest-framework.org/topics/documenting-your-api/)
- [Awesome Django REST Framework (GitHub)](https://github.com/encode/django-rest-framework)
- [drf-yasg (Swagger for DRF)](https://github.com/axnsan12/drf-yasg)
- [drf-spectacular (OpenAPI 3 for DRF)](https://github.com/tfranzel/drf-spectacular)

---

> **Tip:** Each day, read the official docs for the topic, implement the homework, and commit your code. By Day 21, you'll have a strong foundation in DRF and a portfolio-ready project!
