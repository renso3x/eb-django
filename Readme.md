## Live URL

- http://django-env.eba-pxmucee6.ap-southeast-1.elasticbeanstalk.com/admin/

### Reference

- https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create-deploy-python-django.html#python-django-setup-venv

Run the command the status of your Elastic Beanstalk

- `eb status`

```
  Environment details for: django-env
    Application name: django-tutorial
    ...
    CNAME: eb-django-app-dev.elasticbeanstalk.com
    ...
```

- ADD THE CNAME TO `ALLOWED_HOSTS`

```
ALLOWED_HOSTS = ['eb-django-app-dev.elasticbeanstalk.com']
```

Run `eb deploy`
