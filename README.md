# reactDemo
按照多个教程写的demo

demo1—ReactDOM.render()

demo2,demo3—JSX语法

demo4—组件

demo5—this.props.children(组件的所有子节点)

demo6—PropTypes(验证组件实例的属性是否符合要求)

demo7—获取真实的DOM节点

demo8—getInitialState(定义初始化状态),this.state(读取属性),this.setState(修改属性)

demo9—表单

    表单原件的问题：
    1.用value，改成dafaultValue否则改变不了value值
    2.用checked，改成defaultChecked

demo10—组件的生命周期
    
    三个状态
    Mounting：已插入真实 DOM
    Updating：正在被重新渲染
    Unmounting：已移出真实 DOM
    
    六种处理函数
    componentWillMount()
    componentDidMount()
    componentWillUpdate(object nextProps, object nextState)
    componentDidUpdate(object prevProps, object prevState)
    componentWillUnmount()
    componentWillReceiveProps() 组件参数更新
    
demo11—Ajax

#react原生事件和合成事件：

合成事件—在jsx中直接绑定的事件

    <a ref="aaa" onClick = {}><a>

原生事件—通过js原生代码绑定的事件
 
 
 阻止事件冒泡
 
    1、阻止合成事件之间的冒泡，用e.stopPropagation()
     
    2、阻止合成事件于最外层document上的事件间的冒泡，用e.nativeEvent.stopImmediatePropagation()
    
    3、阻止合成事件与除最外层document上的原生事件上的冒泡，通过判断e.target来避免
    