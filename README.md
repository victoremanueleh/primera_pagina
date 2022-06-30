# INICIO DE LA PAGINA  #Nuevo inicio  

Este es el abance del contenido

``` ruby
Etiqueta para codigo
```

See [installation instructions][install] on the wiki for more info.

ℹ️ Puedes acceder a mi perfil para ver informacion acerca de mi persona. [Mi perfil](https://www.facebook.com/victoremanueleh)

## En esta parte se muestra una consepto diferente de codigo

``` ruby
## perform a paginated query:
@posts = Post.paginate(page: params[:page])
# or, use an explicit "per page" limit:
Post.paginate(page: params[:page], per_page: 30)
## render page links in the view:
<%= will_paginate @posts %>
```
Pequeña descripcion del codigo implementado de la nueva pagina en git

``` ruby
# for the Post model
class Post
  self.per_page = 10
end
# set per_page globally
WillPaginate.per_page = 10
```
La nueva estrategia de codigo abierto

``` ruby
# paginate in Active Record now returns a Relation
Post.where(:published => true).paginate(:page => params[:page]).order('id DESC')
# the new, shorter page() method
Post.page(params[:page]).order('created_at DESC')
```

[intagram](https://instagram.com/victoremanueleh)

Happy paginating.
