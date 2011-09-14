Django Trainingen
=================

Learning Django
------------
1. Read the [Django Book][book], it is excellent
2. Read the [Django docs][docs]
3. [django-users mailing list][django-users]
4. [django-developers mailing list][django-developers]
5. irc: #django
6. DjangoCons and [Django Meetings][meetings]
7. [contribute?][contribute]

[book]:http://www.djangobook.com/en/2.0/
[docs]:https://docs.djangoproject.com/en/1.3/
[django-users]:http://groups.google.com/group/django-users
[django-developers]:http://groups.google.com/group/django-developers
[meetings]:http://wiki.python.org/moin/DjangoMeetingNL
[contribute]:https://docs.djangoproject.com/en/1.3/#the-django-open-source-project

Recommendations
---------------
1. [Django packages][packages]
2. [Django snippets][snippets]
3. [Django people][people]
4. [Github][github]

[snippets]:http://djangosnippets.org/
[packages]:http://djangopackages.com/
[people]:http://djangopeople.net/
[github]:https://github.com

Useful shortcuts
----------------
1. [render][render], since 1.3, usage: 
    from django.shortcuts import render
    render('my_template.html', context')
    # render() is the same as a call to render_to_response() with a context_instance argument that forces the use of a RequestContext.

2. [redirect][redirect], since 1.1, usage:      
    from django.shortcuts import redirect
    redirect('name')
    # redirects to:
    # 1. an object, with defined get_absolute_url
    # 2. a named url
    # 3. a hardcoded url (relative or full)

3. If objects have public views, always use get_absolute_url
[render]:https://docs.djangoproject.com/en/1.3/topics/http/shortcuts/#render
[redirect]:https://docs.djangoproject.com/en/1.3/topics/http/shortcuts/#redirect

What’s new in Django 1.3
------------------------

1. [Class-based views][class-based-views]
2. [Logging][logging]
3. [Extended static files handling][static]

What’s new in Django 1.2
------------------------
1. [Improved CSRF protection][csrf]
2. [Messages framework][messages]
3. [Relaxed requirements for usernames][usernames]
4. [Email backends][email backends]
5. [“Smart” if tag][if]
6. [Improved localization][l10n]
7. [readonly_fields in ModelAdmin][readonly]
8. [JavaScript-assisted handling of inline related objects in the admin][inline]

Ad 6. in settings.py:

    USE_I10N = True 

[class-based-views]:https://docs.djangoproject.com/en/1.3/topics/class-based-views/
[logging]:https://docs.djangoproject.com/en/1.3/topics/logging/
[static]:https://docs.djangoproject.com/en/1.3/ref/contrib/staticfiles/
[csrf]:https://docs.djangoproject.com/en/1.3/ref/contrib/csrf/
[messages]:https://docs.djangoproject.com/en/1.3/ref/contrib/messages/
[usernames]:https://docs.djangoproject.com/en/dev/releases/1.2/#relaxed-requirements-for-usernames
[email backends]:https://docs.djangoproject.com/en/dev/topics/email/#topic-email-backends
[if]:https://docs.djangoproject.com/en/dev/releases/1.2/#smart-if-tag
[l10n]:https://docs.djangoproject.com/en/dev/topics/i18n/localization/#format-localization
[readonly]:https://docs.djangoproject.com/en/dev/releases/1.2/#readonly-fields-in-modeladmin
[inline]: https://docs.djangoproject.com/en/dev/releases/1.2/#javascript-assisted-handling-of-inline-related-objects-in-the-admin


Middleware and context processors
------------------------

1. [Middleware][middleware]
2. [Context processors][context_processors]

### Examples
1. [django.contrib.auth.AuthenticationMiddleware][auth-middleware]
2. [django.contrib.auth.context_processors][auth-processor]

[middleware]:https://docs.djangoproject.com/en/1.3/topics/http/middleware/
[context_processors]:https://docs.djangoproject.com/en/dev/ref/templates/api/#writing-your-own-context-processors

[auth-middleware]:https://github.com/django/django/blob/master/django/contrib/auth/middleware.py
[auth-processor]:https://github.com/django/django/blob/master/django/contrib/auth/context_processors.py


Github
------
https://github.com/

[For example: django-debug-toolbar][django-debug-toolbar]
[django-debug-toolbar]:https://github.com/django-debug-toolbar/django-debug-toolbar

[Creating a repository][create-git-repo]
[create-git-repo]:http://help.github.com/create-a-repo/

Git and github
--------------
### Set up git
    git config --global user.name "Wim Feijen"
    git config --global user.email wim@go2people.nl
        
### Next steps:
    mkdir Django-Trainingen
    cd Django-Trainingen
    git init
    touch README
    git add README
    git commit -m 'first commit'
    git remote add origin git@github.com:wimfeijen/Django-Trainingen.git
    git push -u origin master

### Upload ssh key?
https://github.com/account/ssh
      
### Existing Git Repo?
    cd existing_git_repo
    git remote add origin git@github.com:wimfeijen/Django-Trainingen.git
    git push -u origin master

Git
---

### Updating the repo
- git add
- git status
- git commit -m 'Description of the change'
- git push

### Creating a branch
- git clone

### Update your branch
- git pull


Markdown
--------
[Basics][markdown-basics]
[markdown-basics]:http://daringfireball.net/projects/markdown/basics

[Syntax][markdown-syntax]
[markdown-syntax]:http://daringfireball.net/projects/markdown/syntax

Likes
-----
- File and image handling (django-photologue)
- User registration (django-registration) and sessions
- Testing (django-debug-toolbar, nose, werkzeug, gdb, eclipse)
- Database migrations (south)
- Automated deployments (fabric, zc.buildout)
- Caching (memcached)
- Webservices (django-tastypie)
- Facebook / social integration (django-socialregistration)
- Pagination (endless-pagination)
- IDEAL payments (django-mollie) 

Tips
----

- [IDE][ide]
- [gedit][gedit]

[ide]:http://groups.google.com/group/django-users/browse_thread/thread/6705476b48c146b6/b02b6b5c09a3af16?q=gedit&lnk=ol&
[gedit]:http://www.micahcarrick.com/gedit-as-a-django-ide-for-linux.html

About the author
----------------

** Wim Feijen **
- [Go2People Websites][go2people]
- [LinkedIn][linkedin]
- [Twitter][twitter]

[go2people]:http://www.go2people.nl
[linkedin]:http://www.linkedin.com/profile/view?id=10669566
[twitter]:http://twitter.com/#!/wimfeijen



