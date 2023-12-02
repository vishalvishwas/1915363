function prompt {

    $dir = (Get-Location).Path
    $hostname = $env:COMPUTERNAME
    $datetime = Get-Date -Format "dd-MM-yyyy HH:mm:ss"
    $white = [char]27 + "[0m"
    $red = [char]27 + "[31m"
    $green = [char]27 + "[32m"
    $blue = [char]27 + "[34m"
    $yellow = [char]27 + "[33m"
    $purple = [char]27 + "[35m"
    $cyan = [char]27 + "[36m"
    
    Write-Host ("[${green}vishal@${purple}$hostname${white}]-[${blue}$dir${white}]-[${yellow}$datetime${white}]")
    "${cyan}> ${red}"
    
}
