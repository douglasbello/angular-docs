## Componentes

Componentes são a principal construção de blocos para aplicações Angular. Cada componente consiste
em: <br>

<li>Um template HTML que declara o que a página irá renderizar.</li>
<li>Uma classe TypeScript que define o comportamento.</li>
<li>Um seletor CSS que define como o componente é usado em um template.</li>
<li>Opcionalmente, estilos CSS aplicados ao template.</li>
<br>

### Criando um componente utilizando o Angular CLI
Para criar um componente usando o Angular CLI:
<br>

<ol>
<li>No terminal, navegue até o diretório que está sua aplicação.</li>
<li>Rode o <b>ng generate component "component-name".</b></li>
</ol>

Por padrão, esse comando cria os seguintes:
<ul>
<li>Um diretório com o mesmo nome do componente.</li>
<li>Um arquivo componente, <b>component-name.component.ts</b></li>
<li>Um arquivo template, <b>component-name.component.html</b></li>
<li>Um arquivo CSS, <b>component-name.component.css</b></li>
<li>Um arquivo de especificação de testes, <b>component-name.component.spec.ts</b></li>
</ul>

<hr>

### Especificando o CSS selector do componente

Cada componente requer um seletor CSS. Um seletor instrui o Angular a instanciar um componente em qualquer lugar
que ache a tag correspondente ao template HTML. Por exemplo. considere um componente `hello-world.components.ts`
que define um seletor como `app-hello-world`. Esse seletor instrui o Angular a instanciar esse componente qualquer
vez que a tag `<app-hello-world>` aparece em um template.

<br>

Especifique um seletor de componente adicionando a propriedade `selector` dentro da anotação `@Component`.

```
@Component({
  selector: 'app-component-overview',
})
```

<hr>

### Definindo o template de um componente

O template é um bloco de HTML que diz ao Angular como renderizar o component na sua aplicação. Defina um template
para o seu componente com um dos de dois jeitos: referenciando um arquivo externo, ou diretamente dentro do componente. 

Quando trabalhando com uma aplicação baseada em <i>NgModules</i>, os componentes precisam ser adicionados ao `@NgModule`.
Para embutir um componente em um modulo, adicione ele ao array de declarations dentro da anotação `@NgModule`.

<br>

```
import { ComponentOverviewComponent } from './component-overview.component';

@NgModule({
  declarations: [
    ComponentOverviewComponent,
  ]
})
```
