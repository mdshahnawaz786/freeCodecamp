Answer - 1 --> class MyComponent extends React.Component { constructor(props) { super(props); this.state = { name: 'freeCodeCamp' } } render() { // change code below this line const name = this.state.name; // change code above this line return (

    <h1>{name}</h1>
    
  </div>
);
} };

Answer - 2 --> class MyComponent extends React.Component { constructor(props) { super(props); this.state = { name: 'freeCodeCamp' } } render() { // change code below this line const name = this.state.name; // change code above this line return (

    <h1>{name}</h1>

  </div>
);
} };

Answer - 3 --> class MyComponent extends React.Component { constructor(props) { super(props); this.state = { name: 'Initial State' }; this.handleClick = this.handleClick.bind(this); } handleClick() { // change code below this line this.setState({ name: 'React Rocks!' }); // change code above this line } render() { return (

Click Me
{this.state.name}
); } };
Answer - 4 --> class MyComponent extends React.Component { constructor(props) { super(props); this.state = { visibility: false }; this.toggleVisibility = this.toggleVisibility.bind(this); } toggleVisibility() { this.setState(state => ({ visibility: !state.visibility })); } render() { if (this.state.visibility) { return (

Click Me
Now you see me!
); } else { return (
Click Me
); } } };
Answer - 5 --> (class MyApp extends React.Component { constructor(props) { super(props); this.state = { name: 'CamperBot' } } render() { return (

); } }; class Navbar extends React.Component { constructor(props) { super(props); } render() { return (
Hello, my name is: {this.props.name}
); } };
)
