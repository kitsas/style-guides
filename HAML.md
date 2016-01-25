# HAML Style Guide

Don't use interpolation if not needed
```
# Bad
%h1 #{t('views.backoffice.edit')}

# Good
%h1= t('views.backoffice.edit')

# Good
%h1= "#{t('views.backoffice.edit')} with some text after"
```


Don't use rocket arrows
```
# Bad
%div{ class => 'button' }

# Good
%div{ class: 'button' }
```

Put spaces between curly braces
```
# Bad
%div{class: 'button'}

# Good
%div{ class: 'button' }
```

Use single quotes if there is no interpolation
```
# Bad
%div{ class: "button" }

# Good
%div{ class: 'button' }
%div{ class: "button button--#{color}" }
```
