# Creating NodeJS app without installing node locally

## build image
```docker build -t nodenoinstall .```

## run container without closing replace ${pwd} with %cd% if cmd instead of powershell
```docker run -v ${pwd}:/app -td --name noinstallnode nodenoinstall```

### enter bash
```docker exec -it noinstallnode /bin/sh```

## npm install anything will appear in local files

```npm install express```

## exit bash
```exit```