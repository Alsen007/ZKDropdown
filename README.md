ZKDropdown
==========

A drop down list control for iOS. iPhone version only at this stage

## TODO

<pre>
 * Add this porject to CocoaPods
 * Adding support to iOS 7
</pre>

## Useage

Just use it in code like:

<pre>drop = [[ZKDropdown alloc] initDropdownToObject:self.moveableBtn 
                                WithKeys:@[@"1234", @"Number 2", @"1234", @"Number 2"] 
                                andValues:@[@"a", @"b", @"c", @"d"] 
                                withType:ZKSelectionModeSingle 
                                complete:^(BOOL isSelectedMade, id key, id value) {
                                        if (isSelectedMade) {
                                                [self.moveableBtn setTitle:key forState:UIControlStateNormal];
                                        }
                                }];
</pre>

## LICENSE

The MIT License (MIT)

Copyright (c) 2014 Zack Chung

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
