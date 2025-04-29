# sf-gha-release

Github action for å release flxbl artifacts

## Requirements

`sfp cli` må være installert

Actionen trenger disse tilgangene:

```yaml
permissions:
    contents: read
    packages: read
```

## Usage

<!-- Start usage -->
```yaml
- uses: navikt/sf-gha-release@main
    # 
    # Required: false
    # Default: ''
    
    with:
        # Optional: Specify a release tag to use instead of the latest
        # Required: false
        # Default: ''
        release_tag: ''

        # Optional: Specify the log level
        # Required: false
        # Default: 'INFO'
        loglevel: ''
        
        # Specify the devhub alias
        # Required: true
        # Default: 'devhub'
        devhub_alias: ''
        
        # Specify the target org alias
        # Required: true
        # Default: ''
        target_org_alias: ''

        # Specify the release name prefix
        # Required: true
        # Default: 'sf'
        releaseNamePrefix:
```
<!-- end usage -->

## Henvendelser

Spørsmål knyttet til koden eller prosjektet kan stilles som issues her på GitHub.

## For NAV-ansatte

Interne henvendelser kan sendes via Slack i kanalen #platforce.
