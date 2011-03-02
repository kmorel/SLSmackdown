project(SLSmackdown NONE)

cmake_minimum_required(VERSION 2.8)

include(UseLATEX.cmake)

add_latex_document(SLSmackdown.tex
  BIBFILES SLSmackdown.bib
  )
