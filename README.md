# SwiftIndexDemo
### 11月20练习
* 给tableView添加索引功能，使用其代理方法 sectionForSectionIndexTitle：
```
    func tableView(_ tableView: UITableView, sectionForSectionIndexTitle title: String, at index: Int) -> Int {
        var indexSection : Int = 0
        for i in sections {
            if i == title {
                return indexSection
            }
            indexSection += 1
        }
        return 0
    }
```
