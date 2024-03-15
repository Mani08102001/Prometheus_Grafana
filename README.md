# Prometheus_Grafana

#To get a base64 code  kubectl get secret --namespace default grafana -o jsonpath="{.data.admin-password}"

#To enable base64 to plain text

# function Invoke-Base64Decode {
     param (
         [Parameter(Mandatory=$true)]
         [string]$Base64String
     )

     $decodedBytes = [System.Convert]::FromBase64String($Base64String)
     return [System.Text.Encoding]::UTF8.GetString($decodedBytes)
 }

#To decode    Invoke-Base64Decode "UUR5d3YwZGZYTFlpYVZJWHVwc3ZrNGdVQmpvMVFOallwQ1JpeUE2Mw=="
