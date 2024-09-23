# BaiduBce

Original BCE SDK for .NET, but modified to support with .NET Standard 2.0 and
.NET NativeAOT.

It was originally a component in https://github.com/halalcloud/halalcloud-client.
Due to the Halal Cloud Client will use C++ except the gRPC client part uses
C# for better developing work. This is the reason of this repository existance.

Hope this work can give some help for other developers.

Read https://github.com/baidubce/bce-sdk-dotnet for usage.

## Differences from the original implementation

- Although the original BCE SDK for .NET an open source project, but it seems
  it cannot be compiled successfully, this is why this is based on the ILSpy
  dump from their release binary.
- The original BCE SDK for .NET is only designed for .NET Framework CLR 2.0,
  it's not modern, so this modified version has been adapted to .NET Standard
  2.0 and .NET NativeAOT.
- For supporting Standard 2.0 and .NET NativeAOT, this implementation uses
  Microsoft.Extensions.Logging and System.Text.Json instead of log4net and
  Newtonsoft.Json.

## Documents

- [License](License.md)
