#	@(#)Makefile	8.1 (Berkeley) 6/5/93
# $FreeBSD$

.include <bsd.own.mk>

MAN=	crash.8 \
	diskless.8 \
	intro.8 \
	nanobsd.8 \
	picobsd.8 \
	rc.8 \
	rc.sendmail.8 \
	rc.subr.8 \
	rescue.8 \
	${_uefi.8} \

MLINKS=	rc.8 rc.atm.8 \
	rc.8 rc.d.8 \
	rc.8 rc.firewall.8 \
	rc.8 rc.local.8 \
	rc.8 rc.network.8 \
	rc.8 rc.pccard.8 \
	rc.8 rc.serial.8 \
	rc.8 rc.shutdown.8

.if ${MK_NIS} != "no"
MAN+=	yp.8

MLINKS+=yp.8 NIS.8 \
	yp.8 nis.8 \
	yp.8 YP.8
.endif

.if ${MACHINE_CPUARCH} == "amd64"
_uefi.8= uefi.8
.endif

.include <bsd.prog.mk>
