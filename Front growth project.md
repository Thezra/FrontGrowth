# Front growth project

## Good practices

### Mobile First

- The design must look good on a mobile screen (320px min)
- Light and fast loading
- Buttons must be accessible for touch screens

### Atomic Design

![Por qué usar Atomic Design?](https://static.platzi.com/media/user_upload/0B052198-E473-4908-8866-43780AB15729-f589b505-81e5-4457-a014-793fe19ac768.jpg)

### BEM (Block, Element, Modifier)

- Un **bloque** es **una sección independiente que tiene significado propio por sí solo**. Contiene todos los nodos HTML de una estructura a la que te estés refiriendo.

- Un **elemento** son **porciones más pequeñas internas a un bloque**. Se usa para ir dividiendo el bloque en segmentos más pequeños.

- Un **modificador** sirve para **modificar algunas propiedades de un bloque o elemento**.

```html
<!-- EXAMPLE 1 -->
<div class="block">
    <div class="block__element">Elem 1</div>
    <div class="block__element">Elem 2</div>
    <div class="block__element block__element--modifier">Elem 3</div>
</div>

<!-- EXAMPLE 2 -->
<div class="item item--modifier">
    <div class="item__element">Elem 1</div>
    <div class="item__element">
        <div class="item__another-element">Elem 2</div>
        <div class="item__another-element">Elem 3</div>
    </div>
    <div class="item__element item__element--modifier">Elem 4</div>
</div>
```

```css
// EXAMPLE 1
.block{ color: inherit; }
.block__element{ color: inherit; }
.block__element--modifier{ color: inherit; }

// EXAMPLE 2
.item{ color: inherit; }
.item--modifier{ color: inherit; }
.item__element{ color: inherit; }
.item__element--modifier{ color: inherit; }
.item__another-element{ color: inherit; }
```

```scss
// EXAMPLE 1
.block{ 
    color: inherit;
    &__element{
        color: inherit;
        &--modifier{ 
            color: inherit;
        }
    }
}

// EXAMPLE 2
.item{ 
    color: inherit;
    &--modifier{
        color: inherit;
    }
    &__element{
        color: inherit;
        &--modifier{
            color: inherit;
        }
    }
    &__another-element{
        color: inherit;
    }
}
```

### Technical SEO

### Naming conventions

#### Variables

- Names are case-sensitive, lowercase and uppercase are different.
- Start variable names with a letter, use `camelCase` for names.
- Variable names should be self-descriptive, describing the stored value.
- Boolean variables are usually prefixed with `is` or `has`.

#### Functions

- Names are case-sensitive, lowercase and uppercase are different.
- Start function names with a letter, use `camelCase` for names.
- Use descriptive names, usually verbs in the imperative form.
- Common prefixes are `get`, `make`, `apply` etc.
- Class methods follow the same rules.

#### Constant

- Names are case-sensitive, lowercase and uppercase are different.
- Define constants at the top of your file, function or class.
- Sometimes `UPPER_SNAKE_CASE` is used, while other times plain `camelCase`.

#### Classes

- Names are case-sensitive, lowercase and uppercase are different.
- Start class names with a capital letter, use `PascalCase` for names.
- Use descriptive names, explaining the functionality of the class.
- Components, which are used in frontend frameworks follow the same rules.

#### Private

- Prefix any variable or function with `_` to show intention for it to be private.
- As a convention, this will not prevent other parts of the code from accessing it.

### GitFlow

--------------------------------------------------------------------

## Proyecto 1: To-do List

### Description

#### Base

Creation of a web page that allows to keep track of pending, started and finished tasks. It must allow to drag and drop the the tasks depending on the current state. The web page should have a register and login option to keep the board info on a DB by user.

#### Extras

- Being able to create boards by topics or tags
- Being able to put limit time or date
- Create a system to notify when the task is about to finish

### Definition of Done (DoD)

- [ ] dasda
- [ ] Fulfills good practices
- [ ] Unit testing
- [ ] Functional testing



## Project 2: Movies Database

### Description

### Definition of Done (DoD)



## Project 3: Card memory game

### Description

### Definition of Done (DoD)

