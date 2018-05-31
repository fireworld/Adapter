# Android Extension

便捷工具类， 同时为另外几个项目提供基础依赖，后续可能会添加更多功能。

## 主要文件

| 文件名称          | 摘要                                                         |
| ----------------- | ------------------------------------------------------------ |
| ViewHolder        | 免去 findViewById, 提供快捷操作各种 View 的方法。            |
| AdapterViewHolder | 继承自 ViewHolder, 主要为后续的 ListView 和 RecyclerView 的通用 Adapter 提供支持。 |
| IntPair           | 与 android.util.Pair<F, S> 类似，同时实现了 Parcelable 接口。 |
| SimpleTextWatcher | 实现 android.text.TextWatcher 的所有方法，但方法体均为空。   |
| AndroidUtils      | 单位转换、设置全屏、获取屏幕尺寸等方法。                     |

## 使用方法

1. 在项目的 build.gradle 文件中配置仓库地址：

   ```groovy
   allprojects {
   		repositories {
   			...
   			maven { url 'https://jitpack.io' }
   		}
   }
   ```

2. 添加项目依赖：

   ```groovy
   dependencies {
   	        implementation 'com.github.fireworld:AndroidExtension:v1.0.1'
   }
   ```

