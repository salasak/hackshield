cmake_minimum_required (VERSION 2.6)

# Nome do projeto
project(GHPUpdater)

# Gera o RC
configure_file (
  "${PROJECT_SOURCE_DIR}/resource.rc.in"
  "${PROJECT_SOURCE_DIR}/resource.rc"
  )

add_executable(GHPUpdater WIN32
	main.cpp
	resource.rc
	)