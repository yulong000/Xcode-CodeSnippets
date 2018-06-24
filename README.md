# Xcode-CodeSnippets
Xcode的代码块

快捷键   ->    对应的内容

sstrong   ->  
```objective-c
@property (nonatomic, strong) <#class#> *<#name#>;
```
wweak     ->  
```objective-c
@property (nonatomic, weak)   <#class#> *<#name#>;
```
assign    ->  
```objective-c
@property (nonatomic, assign) <#type#> <#name#>;
```
ccopy     ->  
```objective-c
@property (nonatomic, copy)   <#class#> *<#name#>;
```
bbool     ->  
```objective-c
@property (nonatomic, assign) BOOL <#name#>;
```
delegate  ->  
```objective-c
@property (nonatomic, weak)   id <#protocol#> delegate;
```

__weak    ->  
```objective-c
__weak typeof(self) weakSelf;
```
mark      ->  
```objective-c
#pragma mark
```
interface ->
```objective-c
@interface <#class#> ()

@end
```

自定义cell时    ->
```objective-c
+ (instancetype)cellWithTableView:(UITableView *)tableView {
    static NSString *ID = @"<#ID#>";
    <#class#> *cell = [tableView dequeueReusableCellWithIdentifier:ID];
    if(cell == nil) {
        cell = [[<#class#> alloc] initWithStyle:UITableViewCellStyleSubtitle reuseIdentifier:ID];
    }
    return cell;
}

- (instancetype)initWithStyle:(UITableViewCellStyle)style reuseIdentifier:(NSString *)reuseIdentifier {
    if(self = [super initWithStyle:style reuseIdentifier:reuseIdentifier]) {
    
    }
    return self;
}

- (void)setSelected:(BOOL)selected animated:(BOOL)animated {
    [super setSelected:selected animated:animated];
    
}

- (void)layoutSubviews {
    [super layoutSubviews];
    
}



```
