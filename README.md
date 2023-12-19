# how-to-center-align-the-header-text-in-.net-maui-expander
This example demonstrates about how to center align the header text in .NET MAUI Expander (SfExpander).

You can center align the text of the Expander Header in .NET MAUI SfExpander by using the HorizontalTextAlignment and VerticalTextAlignment properties.

XAML:

Set HorizontalTextAlignment and VerticalTextAlignment of the header label to Center.

{% tabs %}
{% highlight xaml tabtitle="MainPage.xaml"%}
<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
             xmlns:syncfusion="clr-namespace:Syncfusion.Maui.Expander;assembly=Syncfusion.Maui.Expander">

<ScrollView BackgroundColor="#EDF2F5">
    <StackLayout>
        <syncfusion:SfExpander>
            <syncfusion:SfExpander.Header>
                <Grid HeightRequest="50">
                    <Label Text="Veg Pizza" TextColor="#495F6E" VerticalTextAlignment="Center" HorizontalTextAlignment="Center"/>
                </Grid>
            </syncfusion:SfExpander.Header>
            <syncfusion:SfExpander.Content>
                <Grid Padding="10,10,10,10" BackgroundColor="#FFFFFF">
                    <Label BackgroundColor="#FFFFFF" HeightRequest="60" Text="Veg pizza is prepared with the items that meet vegetarian standards by not including any meat or animal tissue products." TextColor="#303030" VerticalTextAlignment="Center"/>
                </Grid>
            </syncfusion:SfExpander.Content>
        </syncfusion:SfExpander>
        <syncfusion:SfExpander>
            <syncfusion:SfExpander.Header>
                <Grid HeightRequest="50">
                    <Label Text="Non-veg Pizza" TextColor="#495F6E" VerticalTextAlignment="Center" HorizontalTextAlignment="Center"/>
                </Grid>
            </syncfusion:SfExpander.Header>
            <syncfusion:SfExpander.Content>
                <Grid Padding="10,10,10,10" BackgroundColor="#FFFFFF">
                    <Label Text="Non-veg pizza is prepared by including the meat and animal tissue products." HeightRequest="50" TextColor="#303030" VerticalTextAlignment="Center"/>
                </Grid>
            </syncfusion:SfExpander.Content>
        </syncfusion:SfExpander>
    </StackLayout>
</ScrollView>
{% endhighlight %}
{% endtabs %}
