# ros::init()
    void init(int &argc, char **argv, const std::string& name, uint32_t options = 0)
- parmas  
    names: 节点名称  
初始化ros节点。  

# ros::NodeHandle
类名，句柄。  
When a NodeHandle is constructed, it checks to see if the global node state has already been started.  If so, it increments a global reference count.  If not, it starts the node with ros::start() and sets the reference count to 1.
## 构造函数
    //默认构造函数  
    NodeHandle(const std::string& ns = std::string(), const M_string& remappings = M_string());  
    //拷贝构造函数   
    NodeHandle(const NodeHandle& rhs);  
    //根据父句柄构造当前句柄，并指定命名空间  
    NodeHandle(const NodeHandle& parent, const std::string& ns);  
    NodeHandle(const NodeHandle& parent, const std::string& ns, const M_string& remappings);  

# ros::spin()
    订阅者开始接受话题消息，进入循环，调用callbacks，执行回调函数。

# ros::spinOnce()
