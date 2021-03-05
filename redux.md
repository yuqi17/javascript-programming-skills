这个框架作为全局数据的管理是比较好用的，但是其实定义了很多key反而让编码变得很麻烦。建议保存全局数据的时候采用，可以缓存这些数据提高执行效率。但是对于同步性很高的，无需全局缓存的变量
来说没必要用它。所以在新的react 中有 useReducer，useContext, 也有 useState, useEffect, useRef
