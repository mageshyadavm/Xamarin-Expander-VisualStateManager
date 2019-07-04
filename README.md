# Visual State Manager example of Xamarin.Forms Expander

The appearance of the [SfExpander](https://help.syncfusion.com/cr/cref_files/xamarin/Syncfusion.Expander.XForms~Syncfusion.XForms.Expander.SfExpander.html) can be customized using the following two `VisualStates`:

* Expanded
* Collapsed

```xml
<syncfusion:SfExpander x:Name="expander">
    <syncfusion:SfExpander.Header>
        <Label  Text="Veg Pizza" VerticalTextAlignment="Center"/>
    </syncfusion:SfExpander.Header>
    <syncfusion:SfExpander.Content>
        <Label HeightRequest="50" Text="Veg pizza is prepared with the items that meet vegetarian standards by not including any meat or animal tissue products." VerticalTextAlignment="Center"/>
    </syncfusion:SfExpander.Content>
    <VisualStateManager.VisualStateGroups>
        <VisualStateGroupList>
            <VisualStateGroup>
                <VisualState Name="Expanded">
                    <VisualState.Setters>
                        <Setter Property="HeaderBackgroundColor" Value="Red"/>
                    </VisualState.Setters>
                </VisualState>
                <VisualState Name="Collapsed">
                    <VisualState.Setters>
                        <Setter Property="HeaderBackgroundColor" Value="Green"/>
                    </VisualState.Setters>
                </VisualState>
            </VisualStateGroup>
        </VisualStateGroupList>
    </VisualStateManager.VisualStateGroups>
</syncfusion:SfExpander>
{% endhighlight %}
```

You can also refer our UG documentation to know more about [VSM]().
