# Custom React Hooks Collection

This repository contains a collection of custom React hooks that can be useful in various situations. There are 4 hooks available:

1. useCounter
2. useFetch
3. useForm
4. useTodos

## useCounter

A custom hook for managing a numeric counter with increment, decrement, and reset actions. This hook takes an optional initial value as an argument.

### Usage

```javascript
import { useCounter } from './useCounter';

const CounterComponent = () => {
    const { counter, increment, decrement, reset } = useCounter();

    return (
        // Your JSX code here
    );
};
```

## useFetch

A custom hook for fetching data from an API. This hook takes a URL as an argument and returns the fetched data, loading state, and any errors encountered.

### Usage

```javascript
import { useFetch } from './useFetch';

const DataComponent = () => {
    const { data, isLoading, hasError } = useFetch('https://api.example.com/data');

    return (
        // Your JSX code here
    );
};
```

## useForm

A custom hook for managing form input state. This hook takes an initial form object as an argument and returns the form state, input change handler, and form reset handler.

### Usage

```javascript
import { useForm } from './useForm';

const FormComponent = () => {
    const { formState, onInputChange, onResetForm } = useForm({ name: '', email: '' });

    return (
        // Your JSX code here
    );
};

```

## useTodos

A custom hook for managing a todo list. This hook handles adding, deleting, and toggling todos, as well as maintaining counts for total todos and pending todos.

### Usage

```javascript
import { useTodos } from './useTodos';

const TodoComponent = () => {
    const { todos, todosCount, pendingTodosCount, handleNewTodo, handleDeleteTodo, handleToggleTodo } = useTodos();

    return (
        // Your JSX code here
    );
};


```
