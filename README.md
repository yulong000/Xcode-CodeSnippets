# Xcode-CodeSnippets
Xcode的代码块

快捷键   ->    对应的内容
```objective-c
sstrong   ->  @property (nonatomic, strong) <#class#> *<#name#>;
wweak     ->  @property (nonatomic, weak)   <#class#> *<#name#>;
assign    ->  @property (nonatomic, assign) <#type#> <#name#>;
ccopy     ->  @property (nonatomic, copy)   <#class#> *<#name#>;
bbool     ->  @property (nonatomic, assign) BOOL <#name#>;
delegate  ->  @property (nonatomic, weak)   id <#protocol#> delegate;


__weak    ->  __weak typeof(self) weakSelf;
mark      ->  #pragma mark

interface ->
@interface <#class#> ()

@end


自定义cell时    ->
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
