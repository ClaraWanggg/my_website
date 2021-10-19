# my_website
library(usethis)
use_git_config(user.name = "Clara Wang", user.email = "lwang.mfa2022@london.edu")
usethis::create_github_token()

library(gitcreds)

gitcreds_set()
gitcreds_get()
#> <gitcreds>
#>   protocol: https
#>   host    : github.com
#>   username: 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
#>   password: <-- hidden -->

install.packages("credentials")
library(credentials)

set_github_pat()

        blogdown::new_site(theme = "MarcusVirg/forty", 
          sample = TRUE, 
          theme_example = TRUE,            
          empty_dirs = TRUE,            
          to_yaml = TRUE)





