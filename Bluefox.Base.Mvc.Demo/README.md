#BlueFox.Base.Mvc使用范例
Install-Package BlueFox.Base.Mvc

控制器继承 PubController 后得到

/// <summary>
/// 服务提供器
/// </summary>
protected IServiceProvider ServiceProvider { get; set; }

/// <summary>
/// 获取依赖注入对象
/// </summary>
/// <typeparam name="T"></typeparam>
/// <returns></returns>
protected T GetService<T>()

/// <summary>
/// 返回对象
/// </summary>
/// <returns></returns>
public IActionResult Success()

/// <summary>
/// 返回对象
/// </summary>
/// <param name="data"></param>
/// <returns></returns>
public IActionResult Success<T>(T data)

/// <summary>
/// 返回消息
/// </summary>
/// <param name="msg"></param>
/// <returns></returns>
public IActionResult Success(string msg)

/// <summary>
/// 返回错误
/// </summary>
/// <returns></returns>
public IActionResult Error(string msg)

/// <summary>
/// 返回错误
/// </summary>
/// <returns></returns>
public IActionResult Error(Exception ex)

/// <summary>
/// 返回表格
/// </summary>
/// <typeparam name="T"></typeparam>
/// <param name="list"></param>
/// <param name="count"></param>
/// <returns></returns>
public IActionResult Table<T>(IList<T> list, int count)

/// <summary>
/// 返回表格
/// </summary>
/// <typeparam name="T"></typeparam>
/// <param name="list"></param>
/// <returns></returns>
public IActionResult Table<T>(IList<T> list)

/// <summary>
/// 返回表格
/// </summary>
/// <typeparam name="T"></typeparam>
/// <param name="page"></param>
/// <returns></returns>
public IActionResult Table<T>(PageResult<T> page)

/// <summary>
/// 获取html模板
/// </summary>
/// <param name="dir"></param>
/// <param name="name"></param>
/// <returns></returns>
public IActionResult Template(string dir, string name)