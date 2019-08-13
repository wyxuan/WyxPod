# WyxPod

[![CI Status](https://img.shields.io/travis/wangyongxuan/WyxPod.svg?style=flat)](https://travis-ci.org/wangyongxuan/WyxPod)
[![Version](https://img.shields.io/cocoapods/v/WyxPod.svg?style=flat)](https://cocoapods.org/pods/WyxPod)
[![License](https://img.shields.io/cocoapods/l/WyxPod.svg?style=flat)](https://cocoapods.org/pods/WyxPod)
[![Platform](https://img.shields.io/cocoapods/p/WyxPod.svg?style=flat)](https://cocoapods.org/pods/WyxPod)

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

WyxPod is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'WyxPod'
```

## Author

wangyongxuan, w_yongxuan@163.com

## License

WyxPod is available under the MIT license. See the LICENSE file for more info.

## Des
pod创建：git上创建仓库
组件化：pod lib create podName
git add .
git commit -m "config"
git remote add origin https://github.com/wyxuan/WyxPod.git
git push -u origin master

验证：pod lib lint WyxPod.podspec///pod lib lint WyxPod.podspec --allow-warnings
出现错误：xcrun: error: unable to find utility "simctl", not a developer tool or in PA
xcode偏好locactions中指定command line tools
提交：打tag  查看WyxPod.podspec ：s.version  = '0.1.0'版本
git tag 0.1.0 
git push origin 0.1.0
spec验证： pod spec lint WyxPod.podspec --allow-warnings
发布spec: pod trunk push WyxPod.podspec
[!] You need to register a session first.
执行:  pod trunk me 检查是否有账号
pod trunk register w_yongxuan@163.com "wyxuan" --description='pod的创建'
在执行:pod trunk push WyxPod.podspec/// pod trunk push WyxPod.podspec --allow-warnings
搜索检验：前往这个路径下~/Library/Caches/CocoaPods删除search_index.json文件 ,
                  或者使用终端命令删除:   rm ~/Library/Caches/CocoaPods/search_index.json

