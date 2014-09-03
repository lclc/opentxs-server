# Copyright (c) Monetas AG, 2014

set(cxx-sources
  ServerSettings.cpp
  ConfigLoader.cpp
  AcctFunctor_PayDividend.cpp
  ClientConnection.cpp
  MessageProcessor.cpp
  MainFile.cpp
  UserCommandProcessor.cpp
  Notary.cpp
  Transactor.cpp
  OTServer.cpp
)

add_library(opentxs-server-base ${cxx-sources})

target_link_libraries(opentxs-server-base ${cash} ${core} ${ext})