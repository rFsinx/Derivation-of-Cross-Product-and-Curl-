# Visual-Algebraic-Derivation-of-Divergence-Curl-

## Origin of Curl: the Cross Product

$$\vec{a} = a_x \hat{i} + a_y \hat{j} + a_z \hat{k}, \quad \vec{b} = b_x \hat{i} + b_y \hat{j} + b_z \hat{k}, \quad \vec{c} = \vec{a} \times \vec{b}$$

### Magnitude

$$
|\vec{c}| = |\vec{a} \times \vec{b}| = |\vec{a}| |\vec{b}| \sin\theta
$$

$$
= |\vec{a}| |\vec{b}| \sqrt{1 - \cos^2\theta}
$$

$$
= \sqrt{| \vec{a} |^2 | \vec{b} |^2 - | \vec{a} |^2 | \vec{b} |^2 \cos^2\theta}
$$

$$
= \sqrt{| \vec{a} |^2 | \vec{b} |^2 - (\vec{a} \cdot \vec{b})^2}
$$

$$
= \sqrt{(a_x^2 + a_y^2 + a_z^2)(b_x^2 + b_y^2 + b_z^2) - (a_x b_x + a_y b_y + a_z b_z)^2}
$$

$$
= \sqrt{(a_x b_y - a_y b_x)^2 + (a_y b_z - a_z b_y)^2 + (a_z b_x - a_x b_z)^2}
$$

$$
= \sqrt{c_x^2 + c_y^2 + c_z^2} 
$$

### Orthogonality
$$
\vec{a} \cdot (\vec{a} \times \vec{b}) = 0 \implies a_x c_x + a_y c_y + a_z c_z = 0
$$

$$
\implies \pm ( a_x(a_y b_z - a_z b_y) + a_y(a_z b_x - a_x b_z) + a_z(a_x b_y - a_y b_x) ) = 0
$$


$$
\therefore \quad c_x = \pm (a_y b_z - a_z b_y) \ , \quad c_y = \pm (a_z b_x - a_x b_z) \ , \quad c_z = \pm (a_x b_y - a_y b_x) 
$$

### 2D Projection on $(\hat{u}, \hat{v}) \in \{(\hat{i}, \hat{j}) , \ (\hat{j}, \hat{k}) , \ (\hat{k}, \hat{i})\}$

$$
\vec{a}_{\text{2D}} = a_u \hat{u} + a_v \hat{v} = (|\vec{a}_{\text{2D}}| \cos\alpha)\hat{u} + (|\vec{a}_{\text{2D}}| \sin\alpha)\hat{v}
$$

$$
\vec{b}_{\text{2D}} = b_u \hat{u} + b_v \hat{v} = (|\vec{b}_{\text{2D}}| \cos\beta)\hat{u} + (|\vec{b}_{\text{2D}}| \sin\beta)\hat{v} 
$$

### Trigonometry and Components
$$
\quad |\vec{a}_{\text{2D}}| |\vec{b}_{\text{2D}}| \sin(\beta - \alpha)
$$

$$
= |\vec{a}_{\text{2D}}| |\vec{b}_{\text{2D}}| (\sin\beta \ \cos\alpha - \cos\beta \ \sin\alpha)
$$

$$
= (|\vec{a}_{\text{2D}}| \cos\alpha)(|\vec{b}_{\text{2D}}| \sin\beta) - (|\vec{a}_{\text{2D}}| \sin\alpha)(|\vec{b}_{\text{2D}}| \cos\beta)
$$

$$
= a_u b_v - a_v b_u
$$

### Components of $\vec {c}$
$$
\vec c = \sum | \vec{a}_{\text{2D}} \times \vec{b}_{\text{2D}} | \hat{w}
$$

#### xy-plane
$$
a_x b_y - a_y b_x = c_z \quad (\hat{u}=\hat{i}, \hat{v}=\hat{j}, \hat{w}=\hat{k})
$$

#### yz-plane
$$
a_y b_z - a_z b_y = c_x \quad (\hat{u}=\hat{j}, \hat{v}=\hat{k}, \hat{w}=\hat{i})
$$

#### zx-plane
$$
a_z b_x - a_x b_z = c_y \quad (\hat{u}=\hat{k}, \hat{v}=\hat{i}, \hat{w}=\hat{j}) 
$$

$$
\therefore \quad \vec{c} = (a_y b_z - a_z b_y)\hat{i} + (a_z b_x - a_x b_z)\hat{j} + (a_x b_y - a_y b_x)\hat{k}
$$
