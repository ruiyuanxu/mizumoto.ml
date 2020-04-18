## C#中的IDisposable接口

首先，我们应该明确的一点是：IDisposable是C#用于释放非托管资源的一种接口。
[IDisposable Interface (System)](https://docs.microsoft.com/en-us/dotnet/api/system.idisposable?redirectedfrom=MSDN&view=netframework-4.8)
> Provides a mechanism for releasing unmanaged resources.

重点在于<u>release</u>和<u>unmanaged</u>两点。