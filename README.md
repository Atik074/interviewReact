                       Bootcamp one 
                 subject : React basic concepts 

00.what is react ? 
Ans: React is an efficient, declarative, and flexible open-source JavaScript library for building simple, fast, and scalable frontends of web application.

01. Differentiate between Real DOM and Virtual DOM.?
 
Ans: :Real dom is the  browser’s  representation of  HTML   structures.when user  interacts with website, real dom reflects it and updated html.

 Virtual  dom is an abstraction of real dom and lightweight copy of real dom.when user change any state,virtual dom updates only changable part by diffing algorithm .it has another name reconsilation..


Real dom : every  update requires the browser to recalculate the entire document layout.virtual dom allows for faster updates and improved performance.
	
Virtual DOM is highly flexible and can be used with any programming language. Real DOM is tightly coupled with the browser and can only be manipulated using JavaScript.



02. List some of the major advantages of React  js 
Ans:
i)	 Flexibility due to modular structure
ii)	   Complex app can run high performance for virtual Dom and server side rendering 
iii)	 to learn react you need have basic knowledge of javascript
iv)	Deploying React is fairly easy to accomplish if you have some basic knowledge of JavaScript.
v)	It has reuseable components that saves time  and removes same code repitation 

03)Limitation of React js 

i)	Lack of proper documentation
ii)	Developer speed 
iii)	Jsx complexity
iv)	Problem with SEO
v)	Steep learnig curve: without good knowledge of javascript you can not understand properly react.Virtual dom, jsx syntax, state management of react is painfull,harder concenpt for new  developer
vi)	Boilerplate code: to start new project you need to significant amount of set up and need configuration.set up project structure,installing dependencies,configuration tools such as babel, webpack are count in Boilerplate code.

 04) Why React is best choice ? 
   Ans: 
i)	Easy to learn 
ii)	It helps to build user interface
iii)	Allows writing custome code
iv)	Fast rendering
v)	SEO friendly
vi)	Strong community support
vii)	Available extension


******************************************************
               01.What is JSX, and how does it work? 
	       
Ans:Jsx means javascript XML that is a syntax extension of javascript and valid javascript code .it is a javascript power,  and dynamic value added in jsx file.

Browers does not understand Jsx code . .Babel is a transpiler of js .Jsx code transpile  into javascript code by Babel.then browser understand jsx code .

    02. What are React hooks? Explain the most common React  hooks and their usage. ?
    
    Ans:Hooks are simple javascript function that allow functional component to use state.It can be statefull and manage side effect.

                      Most common in react hooks....

   i)useState: manage state and contains two element.one is     current value and other is  update value that is function.
   
   ii) useEffect:it manage side effect like API call, subscription and more.
   
  iii) useContext:  it retruns a current value from a context
  
  iv) useReducer: it is a alternative of useState hook.it helps with complex state management
  
  v)UseRef:  Returns a ref with current property.

03) Why do you prefer using functional components?
4) 
   Ans: Functional components are simple javascript function that takes a props as an argument and return  a react element to be rendered .
   

    Prefer using functional components
i)	It is easy to learn and code clean & readable
ii)	No require for constructor method
iii)	No concern about “this” keyword
iv)	It is simple than class component
v)	Debugging and testing easier
vi)	It is reuseabl 

******************************************************

Title : Exploring the React component lifecycle: A guide to understanding the different phases.

Introduction: Every React Component has a lifecycle of its own, the lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component’s existence. The definition is pretty straightforward but what do we mean by different stages? A React Component can go through four stages of its life as follows.


A component's life cycle has three main phases: 


the Mounting Phase,
the Updating Phase, 
and the Unmounting Phase.


The Mounting Phase begins when a component is first created and inserted into the DOM. The Updating Phase occurs when a component's state or props change. And the Unmounting Phase occurs when a component is removed from the DOM.


Mounting phase: The mounting phase refers to the period when a component is being created and inserted into the DOM. The mounting phase has three main lifecycle methods that are called in order : 

constructor() : 


The constructor() method is called when the component is first created. You use it to initialize the component's state and bind methods to the component's instance.


render() :


The render() method is responsible for generating the component's virtual DOM representation based on its current props and state. It is called every time the component needs to be re-rendered, either because its props or state have changed, or because a parent component has been re-rendered.

getDerivedStateFromProps() :


getDerivedStateFromProps() is a lifecycle method available in React 16.3 and later versions that is invoked during the mounting and updating phase of a component. It takes two parameters:

props: The updated props for the component.
state: The current state of the component.


Component Updating Phase: This phase occurs when a component's props or state changes, and the component needs to be updated in the DOM.

shouldComponentUpdate() : 


The shouldComponentUpdate()  method is called before a component is updated. It takes two arguments: nextProps and nextState. This method returns a boolean value that determines whether the component should update or not. If this method returns true, the component will update, and if it returns false, the component will not update.


componentWillUpdate() :


componentWillUpdate() is a lifecycle method in React that gets called just before a component's update cycle starts. It receives the next prop and state as arguments and allows you to perform any necessary actions before the component updates.

componentDidUpdate :


The componentDidUpdate() method is a lifecycle method in React that is called after a component has been updated and re-rendered. It is useful for performing side effects or additional operations when the component's props or state have changed.


Component Unmounting Phase : The unmounting phase refers to the lifecycle stage when a component is being removed from the DOM (Document Object Model) and is no longer rendered or accessible. During this phase, React performs a series of cleanup operations to ensure that the component and its associated resources are properly disposed of. The unmounting phase is the last stage in the lifecycle of a React component and occurs when the component is being removed from the DOM tree.

componentWillUnmount() : 


This method is called just before the component is removed from the DOM. It allows you to perform any necessary cleanup, such as canceling timers, removing event listeners, or clearing any data structures that were set up during the mounting phase. After componentWillUnmount() is called, the component is removed from the DOM and all of its state and props are destroyed.




Summary: React components have a life cycle consisting of three phases: Mounting, Updating, and Unmounting. Each phase has specific lifecycle methods that are called at different points in the component's lifecycle.
*****************************************************************************


