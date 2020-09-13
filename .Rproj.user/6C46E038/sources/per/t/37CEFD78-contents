


#' Create a Rmd to support Materialized  frame work
#'
#' @return No return
#' @export
#'
#' @examples none
create_materializedFramework <- function(){
  downloadUrl <- "https://www.dropbox.com/s/oz385kxex63yoa6/MaterializedFramework.zip?dl=1"
  dowload_unzip(downloadUrl)
}


# helpers-----------------------------------

dowload_unzip <- function(downloadUrl){

  filename <- stringr::str_remove(basename(downloadUrl),"\\?[:graph:]+$")

  download.file(
    url=downloadUrl,
    destfile=filename,
    mode='wb'
  )

  unzip(
    zipfile=filename
  )
  # 在R意味著delete file因為已經解壓縮
  unlink(filename)
}

