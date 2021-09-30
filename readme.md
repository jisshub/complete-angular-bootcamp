## injecting to template using event binding and string interpolation

```ts
export class AppComponent {
  title = 'counter-app';

  count: number = 0;

  handleIncrease = () => {
    this.count = this.count + 1;
  };
  handleDecrease = () => {
    if (this.count > 0) {
      this.count = this.count - 1;
    }
  };
  handleReset = () => {
    this.count = 0;
  };
}
```

```html
<div class="container">
  <header>
    <h1>{{title}}</h1>
  </header>

  <main>
    <h2>Current count is : {{count}}</h2>
  </main>

  <button (click)="handleReset()">Reset Count</button>
  <button (click)="handleIncrease()">Increase Count</button>
  <button (click)="handleDecrease()">Decrease Count</button>
</div>
```

## Event binding and string interpolation


