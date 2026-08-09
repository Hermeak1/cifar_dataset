# cifar_dataset

PyTorch 학습용 노트북 모음. 텐서 기초부터 CIFAR-10 데이터셋을 불러와 다루는 것까지 다룹니다.

## 노트북

### `Tensor_lecture.ipynb`
PyTorch 텐서의 기본기.

- 리스트 / NumPy 배열에서 텐서 생성
- `dtype`, `shape`, `device` 등 텐서 속성 확인
- `rand` / `ones` / `zeros`로 초기화
- 인덱싱, 슬라이싱, 연산

### `dataset_cifar.ipynb`
`torchvision`으로 CIFAR-10을 다루는 실습.

- `datasets.CIFAR10`으로 학습/테스트셋 다운로드 (`../.cache`에 저장)
- 10개 클래스 라벨 매핑 (plane, car, bird, cat, deer, dog, frog, horse, ship, truck)
- `matplotlib`으로 샘플 이미지 3×3 그리드 시각화
- `Dataset` / `DataLoader` 사용법

## 실행

```bash
pip install torch torchvision matplotlib numpy
jupyter notebook
```

첫 실행 시 CIFAR-10(약 170MB)이 `../.cache`에 자동으로 내려받아집니다.

## 라이선스

MIT — [LICENSE](LICENSE) 참고.
