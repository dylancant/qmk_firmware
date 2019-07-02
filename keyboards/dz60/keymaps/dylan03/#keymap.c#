#include QMK_KEYBOARD_H

enum custom_keycodes {
  DKEY_A = SAFE_RANGE,
  DKEY_S,
  DKEY_D,
  DKEY_F,
  DKEY_VIM,
  DKEY_GAMMA,
  DKEY_SUPER,
  DKEY_HYPER
};

bool process_record_user(uint16_t keycode, keyrecord_t *record) {
  switch (keycode) {
  case DKEY_A:
    if (record->event.pressed) {
      // when keycode DKEY is pressed
      SEND_STRING(SS_RALT("[")"1a");
    } else {
      // when keycode DKEY is released
    }
    break;
  case DKEY_S:
    if (record->event.pressed) {
      // when keycode DKEY is pressed
      SEND_STRING(SS_LALT("[")"1s");
    } else {
      // when keycode DKEY is released
    }
    break;
  case DKEY_D:
    if (record->event.pressed) {
      SEND_STRING(SS_LALT("[")"1d");
    } else {
    }
    break;
  case DKEY_F:
    if (record->event.pressed) {
      SEND_STRING(SS_LALT("[")"1f");
    } else {
    }
    break;
  case DKEY_VIM:
    if (record->event.pressed) {
      SEND_STRING(SS_LALT("t")"a");
    } else {
    }
    break;
  case DKEY_SUPER:
    if (record->event.pressed) {
      SEND_STRING(SS_LCTRL("x")"@s");
    } else {
    }
    break;
  case DKEY_HYPER:
    if (record->event.pressed) {
      SEND_STRING(SS_LCTRL("x")"@h");
    } else {
    }
    break;
  case DKEY_GAMMA:
    if (record->event.pressed) {
      SEND_STRING(SS_LALT("t")"z");
    } else {
    }
    break;
  }
  return true;
};

const uint16_t PROGMEM keymaps[][MATRIX_ROWS][MATRIX_COLS] = {
        LAYOUT(
	       KC_GRV, KC_1, KC_2, KC_3, KC_4, KC_5, KC_6, KC_7, KC_8, KC_9, KC_0, KC_MINS, KC_EQL, KC_NO, KC_BSLS,
	       KC_TAB, KC_Q, KC_W, KC_E, KC_R, KC_T, KC_Y, KC_U, KC_I, KC_O, KC_P, KC_LBRC, KC_RBRC, KC_BSPC,
	       KC_LCTL, KC_A, KC_S, KC_D, KC_F, KC_G, KC_H, KC_J, KC_K, KC_L, KC_SCLN, KC_QUOT, KC_ENT,
	       KC_LSFT, KC_NO, KC_Z, KC_X, KC_C, KC_V, KC_B, KC_N, KC_M, KC_COMM, KC_DOT, KC_SLSH, KC_RSFT, KC_NO,
	       MO(2), KC_LALT, KC_LGUI, KC_SPC, KC_SPC, KC_SPC, KC_RALT, DKEY_VIM, KC_NO, DKEY_GAMMA, MO(1)),

	LAYOUT(
		KC_GESC, KC_F1, KC_F2, KC_F3, KC_F4, KC_F5, KC_F6, KC_F7, KC_F8, KC_F9, KC_F10, KC_F11, KC_F12, KC_NO, _______,
		_______, RGB_TOG, RGB_MOD, RGB_HUI, RGB_HUD, RGB_SAI, RGB_SAD, RGB_VAI, RGB_VAD, _______, KC_MPLY, KC_BRID, KC_BRIU, RESET,
		_______, _______, _______, _______, _______, _______, KC_MRWD, KC_VOLD, KC_VOLU, KC_MFFD, _______, _______, _______,
		_______, _______, _______, _______, BL_DEC, BL_TOGG, BL_INC, BL_STEP, KC_MUTE, _______, _______, _______, _______, _______,
		_______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______),

	LAYOUT(
	       _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, KC_PGUP,	       
	       _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, KC_UP, _______, _______, _______,
	       _______, _______, _______, _______, KC_RIGHT, _______, KC_LEFT, KC_DOWN, KC_UP, KC_RIGHT, _______, _______, KC_PGDN,
	       _______, _______, _______, _______, _______, _______, KC_LEFT, KC_DOWN, _______, _______, _______, _______, _______, _______,
	       _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______),

	LAYOUT(	       
		_______, M(1), M(2), M(3), M(4), M(5), M(6), M(7), M(8), M(9), M(10), M(11), M(12), KC_NO, _______,
		_______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______,
		_______, DKEY_A, DKEY_S, DKEY_D, DKEY_F, _______, _______, _______, _______, _______, _______, _______, _______,
		_______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______,
		_______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______),

	LAYOUT(
		_______, M(1), M(2), M(3), M(4), M(5), M(6), M(7), M(8), M(9), M(10), M(11), M(12), KC_NO, _______,
		_______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______,
		_______, DKEY_A, DKEY_S, DKEY_D, DKEY_F, _______, _______, _______, _______, _______, _______, _______, _______,
		_______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______,
		_______, _______, _______, _______, _______, _______, _______, _______, _______, _______, _______),

	
	       
};
