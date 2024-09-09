# PROGPOE1
mainWindow:
<Window x:Class="ProgPOE.MainWindow"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:local="clr-namespace:ProgPOE"
        mc:Ignorable="d"
        Title="MainWindow" Height="450" Width="800">
    <Grid>
        <DockPanel>
            <StackPanel DockPanel.Dock="Left" Width="200" Background="LightGray">
                <TextBlock Text="Navigation" FontSize="16" FontWeight="Bold" Margin="10"/>
                <Button Content="Submit Claim" Margin="5" Click="SubmitClaim_Click"/>
                <Button Content="Approve Claims" Margin="5" Click="ApproveClaims_Click"/>
                <Button Content="Upload Documents" Margin="5" Click="UploadDocuments_Click"/>
                <Button Content="Track Claim Status" Margin="5" Click="TrackStatus_Click"/>
            </StackPanel>

            <StackPanel Margin="10">
                <TextBlock Text="Welcome to the CMCS Dashboard" FontSize="24" FontWeight="Bold"/>
                <TextBlock Text="Here you can manage your claims and documents." Margin="5"/>
                <!-- Placeholders for the dashboard overview -->
                <TextBlock Text="Claim Status Overview " Margin="5"/>
            </StackPanel>
        </DockPanel>
    </Grid>
</Window>

uploadDocuments:
<Window x:Class="ProgPOE.UploadDocuments"
        xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
        xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
        xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
        xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
        xmlns:local="clr-namespace:ProgPOE"
        mc:Ignorable="d"
        Title="UploadDocuments" Height="450" Width="800">
    <Grid Margin="10">
        <StackPanel>
            <TextBlock Text="Upload Supporting Documents" FontSize="20" FontWeight="Bold" Margin="0,0,0,10"/>
            <StackPanel Orientation="Horizontal">
                <TextBlock Text="Choose Files:" Width="120"/>
                <Button Content="Browse..." Width="120" Click="BrowseFiles_Click"/>
            </StackPanel>
            <ListBox Name="FilesList" Height="150" Margin="0,10,0,0"/>
            <Button Content="Upload" Width="120" HorizontalAlignment="Center" Click="UploadFiles_Click"/>
        </StackPanel>

    </Grid>
</Window>
