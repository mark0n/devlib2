TOP=..

include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

#=============================
# Build the IOC application

PROD_LIBS += Com

TESTPROD_HOST += pcitest
TESTS += pcitest

pcitest_SRCS += pcitest.c
pcitest_LIBS += epicspci

TESTPROD_HOST += epicsMMIOTest
TESTS += epicsMMIOTest

epicsMMIOTest_SRCS += epicsMMIOTest.c

TESTPROD_HOST += lspcix
lspcix_SRCS += lspcix.c
lspcix_LIBS += epicspci

TESTPROD_HOST += pciio
pciio_SRCS += pciio.c
pciio_LIBS += epicspci

TESTSCRIPTS_HOST += $(TESTS:%=%.t)

#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

