# forma_bonnesPra


support formation : 
- https://inseefrlab.github.io/formation-bonnes-pratiques-R/

ressource : 
- https://eliocamp.github.io/reproducibility-with-r/

format de documentation roxygen2 : 
- https://cran.r-project.org/web/packages/roxygen2/vignettes/roxygen2.html 

# des bouts de code :
config GIT : 
`git config --global credential.helper store`

mise en forme : 
`lintr::lint("script.R")`
`styler::style_file("script.R")`

lecture de ``yaml`` :
`yaml::read_yaml("secrets.yaml")$JETON`

- vérification des arguments dans une fonction : 
``match.arg(b,
            c("moyenne",
              "variance",
              "ecart-type",
              "sd",
              "ecart type")
  )``

- évaluation par cas dans une fonction : 
``  switch(b,
         moyenne = mean(a, ...),
         variance = var(a, ...),
         sd(a, ...)
  )``
