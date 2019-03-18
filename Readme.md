# What's this?
これは.NET Coreの自己完結型の展開 (SCD)のお試しコードです。
自己完結型の展開については、下記の記事を参照してください。

https://docs.microsoft.com/ja-jp/dotnet/core/deploying/index#self-contained-deployments-scd


コードは、ASP.NET CoreのSignalRのチュートリアルを利用しています。

https://docs.microsoft.com/ja-jp/aspnet/core/tutorials/signalr?view=aspnetcore-3.0&tabs=visual-studio-code

linux-x86でリリースした実行パッケージも同梱しています。

実行ファイルは、`bin/Release/netcoreapp3.0/linux-x86/publish/SignalRChat`です。

リリース時のdotnet-sdkのバージョンは`3.0.100-preview3-010431`です。

## How to use？

1. linux-x86環境のマシンに`bin/Release/netcoreapp3.0/linux-x86`を展開します。
2. `linux-x86/publish/SignalRChat`を実行します。
3. ブラウザで`https://<マシンのIP or FQDN>:5000/`にアクセスするとSignalRのデモページが表示されます。
4. 複数のブラウザで、リアルタイムチャットができればOKです。

## Note

今回の場合だと展開したlinux-x64向けのパッケージサイズは約200MBくらいだった。  


