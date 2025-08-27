layout: page
title: "Non-linear System Identification"
date: 2025-08-27

Spring damper system of the following form
$F_s = -ks^p$
$F_d = -f_c\text{sign}(\dot{s})-c_0\dot{s}$

Such that
$m\ddot{s}=-ks^p-f_c\text{sign}(\dot{s})-c_0\dot{s}$

Discrete state-space form (sampling period $T$)
$\dot{s}_{i+1} =  \dot{s}_{i} - \frac{T}{m}(ks_i^p - f_c\text{sign}(\dot{s}_i) - c_0\dot{s}_i)$
$s_{i+1} = s_i + T\dot{s}_i$