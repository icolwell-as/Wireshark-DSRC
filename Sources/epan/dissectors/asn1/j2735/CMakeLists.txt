# CMakeLists.txt
#
# Wireshark - Network traffic analyzer
# By Gerald Combs <gerald@wireshark.org>
# Copyright 1998 Gerald Combs
#
# SPDX-License-Identifier: GPL-2.0-or-later
#

set( PROTOCOL_NAME j2735 )

set( ASN_FILE_LIST
  J2735-AddGrpB.asn
  J2735-AddGrpC.asn
  J2735-BasicSafetyMessage.asn
  J2735-Common.asn
  J2735-CommonSafetyRequest.asn
  J2735-EmergencyVehicleAlert.asn
  J2735-IntersectionCollision.asn
  J2735-ITIS.asn
  J2735-MapData.asn
  J2735-MessageFrame.asn
  J2735-NMEAcorrections.asn
  J2735-NTCIP.asn
  J2735-PersonalSafetyMessage.asn
  J2735-ProbeDataManagement.asn
  J2735-ProbeVehicleData.asn
  J2735-REGION.asn
  J2735-RoadSideAlert.asn
  J2735-RTCMcorrections.asn
  J2735-SignalRequestMessage.asn
  J2735-SignalStatusMessage.asn
  J2735-SPAT.asn
  J2735-TestMessage00.asn
  J2735-TestMessage01.asn
  J2735-TestMessage02.asn
  J2735-TestMessage03.asn
  J2735-TestMessage04.asn
  J2735-TestMessage05.asn
  J2735-TestMessage06.asn
  J2735-TestMessage07.asn
  J2735-TestMessage08.asn
  J2735-TestMessage09.asn
  J2735-TestMessage10.asn
  J2735-TestMessage11.asn
  J2735-TestMessage12.asn
  J2735-TestMessage13.asn
  J2735-TestMessage14.asn
  J2735-TestMessage15.asn
  J2735-TravelerInformation.asn
)

set( EXTRA_DIST
	${ASN_FILE_LIST}
	packet-${PROTOCOL_NAME}-template.c
	${PROTOCOL_NAME}.cnf
)

set( SRC_FILES
	${EXTRA_DIST}
	${EXT_ASN_FILE_LIST}
)

set( A2W_FLAGS -u)

set( EXTRA_CNF
)

ASN2WRS(-d ps)
