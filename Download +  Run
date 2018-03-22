$DownloadUrl = "https://whatever.com/file.exe"
$LocalPath = "c:\wheverever\you\want"
$file = 'yourdownloadfilename.exe';

$down = New-Object System.Net.WebClient
$down.DownloadFile($DownloadUrl,$file);

# This Section copies the installer to a local path defined.
copy-item $file $localpath
$fullfile = $localpath+$file

# This Section starts the installer using and includes any arguments like quiet mode.
start-process -filepath $fullfile
