[Link](https://youtu.be/5ismRwx4ebM)

## Hook - Gắn (gắn vào component)

### Các loại Hooks

```bash
import {
    useState,
    useEffect,
    useLayoutEffect,
    useRef,
    useCallback,
    useMemo,
    useReducer,
    useContext,
    useImperativeHandle,
    useDebugValue
} from 'react'
```

## Sử dụng Hooks, hỗ trợ thêm nhiều tính năng

```bash
function Component() {
    //useState

    const[state, setState] = useState(initState);

    // useEffect

    useEffect(()=> {
        // return...
    },[deps])

    // useLayoutEffect

        useEffect(()=> {
        // return...
    },[deps])

    // useRef

    const ref = useRef()

    //useCallback

    const fn = useCallback(()=> {

    }, [deps])

    //useMemo

    const result = useMemo(()=> {
        // return results for memo
    }, [deps])

    //useReducer

    const [state, dispatch] = useReducer(reducer, initialArg, init)

    //useContext

    const value = useContext(MyContext)

    //useImperativeHandle

    useImperativeHandle(ref, createHandle, [deps])

    //useDebugValue
    useDebugValue(isOnline ? 'Online' : 'Offline');

    return <h1>Hooks</h1>


}
```

### Hooks

1. Chỉ dùng cho funtion component

2. Component đơn giản và trở nên dễ hiểu

   . Không bị chia logic ra như methods trong lifecyle của Class Component

   . Không cần sử dụng 'this'

3. Sử dụng Hooks khi

   . Dự án mới => Hooks

   . Dự án cũ

   . Component mới => Function component + Hooks

   . Component cũ => Giữ nguyên, có thời gian tối ưu sau

   . Logic nghiệp vũ cần sử dụng các tính chất của OOP => Class Component
