# Alertes
## Configuration
```json
'flexible-alerts': {

        style: 'flat',
        note: {
          label: "Information"
        },
        tip: {
          label: "Conseil"
        },
        warning: {
          label: "Avertissement"
        },
        attention: {
          label: "Attention"
        }
      }
```
## Ecriture
> [!NOTE]
> An alert of type 'note' using global style 'callout'.

> [!TIP]
> An alert of type 'tip' using global style 'callout'.

> [!WARNING]
> An alert of type 'warning' using global style 'callout'.

> [!ATTENTION]
> An alert of type 'attention' using global style 'callout'.

## Images
```
![logo](https://docsify.js.org/_media/icon.svg ':size=WIDTHxHEIGHT')

![logo](https://docsify.js.org/_media/icon.svg ':size=50x100') 

![logo](https://docsify.js.org/_media/icon.svg ':size=100') 

<!-- Support percentage --> 
![logo](https://docsify.js.org/_media/icon.svg ':size=10%')
```

## Comment gérer les fichiers à télécharger

Sometimes we will use some other relative path for the link, and we have to tell docsify that we don't need to compile this link. For example:

```
[link](/demo/)
```

It will be compiled to `<a href="/#/demo/">link</a>` and will load `/demo/README.md`. Maybe you want to jump to `/demo/index.html`.

Now you can do that

```
[link](/demo/ ':ignore')
```

You will get `<a href="/demo/">link</a>`html. Do not worry, you can still set the title for the link.

```
[link](/demo/ ':ignore title')

<a href="/demo/" title="title">link</a>
```