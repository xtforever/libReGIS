CC=gcc
CFLAGS=
# $(wildcard *.c)
FILES=dot_v.c \
draw_abs.c \
draw_arc.c \
draw_box.c \
draw_box_fill.c \
draw_circle.c \
draw_circle_fill.c \
draw_free.c \
draw_intensity.c \
draw_line_abs.c \
draw_line_rel.c \
draw_mode.c \
draw_ofs.c \
draw_pattern.c \
draw_pixel_abs.c \
draw_pixel_rel.c \
draw_rel.c \
draw_text.c \
draw_unarc.c \
draw_unbox.c \
draw_unbox_fill.c \
draw_uncircle.c \
draw_uncircle_fill.c \
draw_unline_abs.c \
draw_unline_rel.c \
draw_unpixel_abs.c \
draw_unpixel_rel.c \
identity_m.c \
mult_m.c \
mult_v.c \
projection_opengl_m.c \
projection_w3woody_m.c \
rotx_m.c \
roty_m.c \
rotz_m.c \
scale_m.c \
scale_v.c \
shear_m.c \
translate_m.c \
unit_v.c \
window_clear.c \
window_close.c \
window_new.c 

OFILES:=$(FILES:.c=.o)  

libregis.a: ${OFILES}
	$(AR) $(ARFLAGS) $@ $^
	ranlib $@
clean:
	$(RM) *.o
	$(RM) libregis.a

install:
	install -m 755 -D ReGIS.h ../include/ReGIS.h
	install -m 755 -D libregis.a ../lib/libregis.a
