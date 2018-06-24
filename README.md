# Xcode-CodeSnippets
Xcode的代码块

快捷键       对应的内容
```objective c
sstrong   ->  @property (nonatomic, strong) <#class#> *<#name#>;\<br>
wweak     ->  @property (nonatomic, weak)   <#class#> *<#name#>;\<br>
assign    ->  @property (nonatomic, assign) <#type#> <#name#>;\<br>
ccopy     ->  @property (nonatomic, copy)   <#class#> *<#name#>;\<br>
bbool     ->  @property (nonatomic, assign) BOOL <#name#>;\<br>
delegate  ->  @property (nonatomic, weak)   id <#protocol#> delegate;\<br>
__weak    ->  __weak typeof(self) weakSelf;\<br>
mark      ->  #pragma mark\<br>

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
