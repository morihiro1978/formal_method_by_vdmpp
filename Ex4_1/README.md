# ��4�� ���K���

## 4.1

0�ȏ�105�����̂��鐮��������A�����3�A5�A7�Ŋ������]������ꂼ��a�Ab�Ac�Ƃ���B
���̂Ƃ��Aa�Ab�Ac���猳�̐������߂�֐��� `calculate` �Ƃ���B
�����ŁA3�A5�A7�̍ŏ����{����105�ł��邱�Ƃ���A�����𖞂������͕K��1�������݂���B

---

### (a)

�֐��{�̂̒�`�� `is not yet speified` �Ƃ����`�ŁA�֐� `calculate` �̉A��`��^����B
��������ɂ���āA�߂�l����ӂɒ�܂�悤�ɕK�v�\���ȏ�����^����悤�ɂ���B
�܂��A���O�������K�v�ƍl�����Ȃ�Ί܂߂�悤�ɂ���B

#### ��

```vdm
public calculate: nat * nat * nat -> nat
calculate(a, b, c) == is not yet specified
pre
  a < 3
  and b < 5
  and c < 7
post
  RESULT < 105
  and RESULT mod 3 = a
  and RESULT mod 5 = b
  and RESULT mod 7 = c
```

�u0�ȏ�v��\������Ƃ��A`nat`�^�ŋ������邱�Ƃ��ł��邵�A`int`�^�Ǝ��O/���������g�ݍ��킹�ċ������邱�Ƃ��ł���B
VDM++�̃R�[�h��݌v���Ƃ��čl�����Ƃ��A�ǂ����������c���������ɂ���Č���ł���B

#### �]�k

���O/����������s�\�����ƁA������z��`�i�����j�ł��e�X�g�ɍ��i�����Ƃ��āA�\�[�g�֐����ǂ���������B
�\�[�g�֐��̎�������Ƃ��āu�l�������ɕ���ł��邱�Ɓv���`�����ꍇ�A���͂Əo�͂��ʂ̐����̏W���ł��u�d�l�ǂ���v�Ƃ݂Ȃ����B

---

### (b)

���́u�����āv�͕S�܌��Z�ƌĂ΂�Ă���A`70 * a + 21 * b + 15 * c` ���v�Z���A105�����񂩈�����0�ȏ�105�����ɂȂ�悤�ɂ���Ό��̐��������邱�Ƃ��m���Ă���B
�܂� `70 * a + 21 * b + 15 * c` �� `105` �Ŋ������]�肪���߂鐔�ł���B
�֐� `calculate` �̗v��`��^����B

#### ��

```vdm
public calculate: nat * nat * nat -> nat
calculate(a, b, c) ==
  return (70 * a + 21 * b + 15 * c) mod 105
pre
  a < 3
  and b < 5
  and c < 7
post
  RESULT < 105
  and RESULT mod 3 = a
  and RESULT mod 5 = b
  and RESULT mod 7 = c
```
