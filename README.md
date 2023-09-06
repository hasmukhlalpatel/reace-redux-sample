# react redux sample

```javascript
import { createStore  } from "redux";

const  initialState = {

}

export default (state = initialState, { type, payload }) => {
    switch (type) {

    case typeName:
        return { ...state, ...payload }

    default:
        return state
    }
}

const reducer = (state = initialState, { type, payload })=>{
    switch (type) {

        case "Add":
            return { ...state, ...payload }
            break;
        case "Add":
            return { ...state, ...payload }
            break;
        default:
            return state
        }
}

const store = createStore(reducer, initialState);

store.subscribe(()=>{
    console.log(`store updated ${store.getState()}`);
});

store.dispatch({type:"ADD", payload:100 });

store.dispatch({type:"ADD", payload:100 });
```
