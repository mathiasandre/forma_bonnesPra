# forma_bonnesPra


support formation : 
- https://inseefrlab.github.io/formation-bonnes-pratiques-R/

ressource : 
- https://eliocamp.github.io/reproducibility-with-r/


# des bouts de code :
config GIT : 
`git config --global credential.helper store`

mise en forme : 
`lintr::lint("script.R")`
`styler::style_file("script.R")`

lecture de ``yaml`` :
`yaml::read_yaml("secrets.yaml")$JETON`

dans une fonction : 
``match.arg(b,
            c("moyenne",
              "variance",
              "ecart-type",
              "sd",
              "ecart type")
  )``
